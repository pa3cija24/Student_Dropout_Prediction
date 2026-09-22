# Klasifikacija študentskega izpisa

## Opis naloge

Napoved osipa (izpisa) študentov na podlagi njihovih osebnih, socialnih in akademskih značilnosti. V nalogi so razviti in primerjani štirje modeli strojnega učenja:
- Odločitveno drevo
- Naključni gozd
- Gradient Boosting
- Metoda podpornih vektorjev (SVM)

Cilj je identificirati ključne napovedne spremenljivke ter oceniti uspešnost in uporabnost posameznih modelov pri zgodnjem zaznavanju tveganja za izpis.

## Podatki

Uporabljen je podatkovni nabor **Student Dropout Prediction Dataset**, dostopen na [Kaggle](https://www.kaggle.com/datasets/meharshanali/student-dropout-prediction-dataset/data). Vsebuje 19 značilk in 10.000 instanc (študentov). CSV datoteka s podatki je priložena v tem repozitoriju (`student_dropout.csv`).

## Vsebina repozitorija

| Datoteka | Opis |
|---|---|
| `student_dropout.csv` | Podatkovna množica |
| `student_dropout_prediction.ipynb` | Jupyter notebook s predprocesiranjem, modeli in rezultati |
| `seminarska.pdf` | Pisno poročilo seminarske naloge |

## Povzetek rezultatov

Vsi modeli so dosegli natančnost med 72 % in 83 %, pri čemer je model **Random Forest** dosegel najbolj uravnotežene rezultate med preciznostjo in priklicem, **Gradient Boosting** pa najboljšo splošno ločevalno sposobnost (ROC-AUC = 0.813). Zaradi neuravnoteženosti ciljne spremenljivke (Dropout) so vsi modeli bolje napovedovali študente, ki so nadaljevali študij, kot tiste, ki so ga opustili.

## Viri

Celoten seznam virov je na voljo v PDF poročilu (poglavje Literatura in viri).
