



**Kursa darbs Praktiskā mašīnmācīšanās un prognozēšanas modeļi kursā**

## Autora informācija
* **Autors:** Jānis Paplavskis
* **Datums:** 2026. gada 26. maijs
* **Projekta veids:** Kursa / praktiskais darbs

---

## Projekta apraksts un mērķis
Šī projekta mērķis ir izstrādāt un salīdzināt mašīnmācīšanās modeļus bankas klientu aizplūšanas (*churn*) prognozēšanai. Savlaicīga klientu aiziešanas identificēšana ļauj bankas mārketinga un klientu noturēšanas nodaļām veikt preventīvas darbības (īpaši piedāvājumi, bonusi), tādējādi optimizējot resursus un samazinot finanšu zaudējumus.

Projekts aptver pilnu datu zinātnes dzīves ciklu:
1. **W1–W3 Sintēze:** Iepriekšējo nedēļu rezultātu apkopošana (Klasifikācija, Regresija, Klasterizācija ar K-Means).
2. **Datu pirmapstrāde:** Trūkstošo vērtību aizpildīšana (`SimpleImputer`), kategorisko pazīmju kodēšana (`OneHotEncoder`) un skaitlisko pazīmju mērogošana (`StandardScaler`).
3. **Modeļu izstrāde:** Loģistiskā regresija (`LogisticRegression`), gadījuma meži (`RandomForestClassifier`) un gradienta pastiprināšana (`GradientBoostingClassifier`).
4. **Hiperparametru optimizācija:** Labāko parametru piemeklēšana, izmantojot `GridSearchCV` un k-kārtu krosvalidāciju (`StratifiedKFold`).
5. **Rezultātu analīze:** Modeļu izvērtēšana pēc *F1-score*, *Precision*, *Recall* un kļūdu matricas (*Confusion Matrix*).

### Galvenie secinājumi
* Fināla klasifikācijas modelis sasniedza **90% Precision** klasei *Aiziet*, kas nozīmē, ka banka gandrīz nemaz netērēs resursus veltīgi lojālo klientu segmentam.
* Mazākuma klases **F1-score sasniedza 0.73**, kas ir būtisks uzlabojums salīdzinājumā ar bāzes modeli.

## Instalācija un vides sagatavošana

Lai palaistu šo projektu lokāli, izpildiet šādus soļus:

1. **Klonējiet repozitoriju:**
   git clone [https://github.com/jusu-lietotajvards/repozitorija-nosaukums.git](https://github.com/jusu-lietotajvards/repozitorija-nosaukums.git)
  pip install -r requirements.txt
  jupyter notebook week4_homework.ipynb