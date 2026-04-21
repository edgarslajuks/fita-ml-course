# Customer Churn Analysis (Telco)

Šis projekts analizē telekomunikāciju uzņēmuma klientu aiziešanu (churn) un izveido prognozēšanas modeli.

## 🎯 Projekta mērķis

Identificēt galvenos faktorus, kas ietekmē klientu aiziešanu, un sniegt datu balstītus ieteikumus churn samazināšanai.
No biznesa perspektīvas klientu noturēšana ir kritiska, jo jauna klienta piesaiste izmaksā vairāk nekā esošā noturēšana.


---

## 📊 Kas tika izdarīts

- Datu izpēte un analīze (EDA)
- Datu tīrīšana (TotalCharges konvertācija un trūkstošo datu apstrāde)
- Vizualizācijas:
  - Churn pēc līguma veida
  - Churn pēc interneta pakalpojuma
  - Mēneša maksa vs churn
- Feature encoding (get_dummies)
- Train/Test split
- Logistic Regression modelis

---

## 📈 Galvenie rezultāti

- ~26.6% klientu pamet uzņēmumu
- Sākotnējais modelis: accuracy ~82%
- Balanced modelis: accuracy ~78%, recall churn klientiem ~79%
- Modelis labi identificē stabilos klientus, bet churn klientu prognozēšana ir izaicinošāka

---

## 🔍 Galvenie atklājumi

- Month-to-month klientiem ir visaugstākais churn
- Fiber optic klientiem ir augstāks churn nekā DSL
- Klienti ar augstāku MonthlyCharges biežāk aiziet

---

## 💼 Biznesa secinājumi

- Fokusēties uz month-to-month klientu noturēšanu
- Izstrādāt īpašus piedāvājumus Fiber optic segmentam
- Uzraudzīt klientus ar augstām mēneša izmaksām

---

## 🛠️ Tehnoloģijas

- Python
- Pandas
- Seaborn / Matplotlib
- Scikit-learn

---

## 📂 Projekta struktūra
week4/
├── telco_analysis.ipynb
├── WA_Fn-UseC_-Telco-Customer-Churn.csv

## 🚀 Nākamie uzlabojumi

- Random Forest / XGBoost modeļi
- Feature importance analīze
- Hyperparameter tuning
- Churn prediction dashboard

