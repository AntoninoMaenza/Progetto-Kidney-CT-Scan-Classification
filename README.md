## Progetto Kidney CT Scan Classification 

Progetto di **classificazione di immagini mediche** su dataset di TC renali, con quattro classi target:  

- **Rene normale**  
- **Cisti**  
- **Tumore**  
- **Calcoli**  

L’obiettivo è applicare tecniche di **Deep Learning** con **transfer learning** per costruire un modello in grado di distinguere le diverse patologie renali.  

---

## 📂 Contenuto del Repository  

- `Progetto-Kidney-CT-Scan-Classification.ipynb` → notebook sviluppato interamente su **Google Colab**  
- `README.md` → descrizione del progetto  

*(Il dataset non è incluso nel repository. Vedi sotto come scaricarlo da Kaggle.)*  

---

## 📥 Download del Dataset  

Il dataset **CT KIDNEY DATASET (Normal, Cyst, Tumor, Stone)** è disponibile su Kaggle al seguente link: 
https://www.kaggle.com/datasets/nazmul0087/ct-kidney-dataset-normal-cyst-tumor-and-stone 
 

Per utilizzarlo in **Google Colab**:  

1. Scaricare il file `.zip` dal link Kaggle.  
2. Caricarlo su Colab (o salvarlo in Google Drive).  
3. Estrarlo nella directory di lavoro:  
   ```python
   !unzip kidney-ct-scan-dataset.zip -d CT-KIDNEY-DATASET-Normal-Cyst-Tumor-Stone

Il notebook assume che i dati si trovino nella cartella:

 ```
/content/CT-KIDNEY-DATASET-Normal-Cyst-Tumor-Stone
 ```

---

## Workflow

- **Preprocessing delle immagini:**
  - Ridimensionamento
  - Equalizzazione dell’istogramma con OpenCV
  - Creazione del DataFrame con path, etichette e dimensioni immagini
  - Caricamento in batch con PyTorch DataLoader

- **Definizione del modello con architetture pre-addestrate:**
  - ResNet50
  - VGG16

- **Training e validazione:**
  - Addestramento del modello
  - Calcolo dell'accuratezza

- **Valutazione finale:**
  - Matrice di confusione
  - Classification report

---

## 📈 Risultati

ResNet50 ha fornito performance migliori rispetto a VGG16.

---

## 🔑 Tecnologie Utilizzate
- Google Colab (GPU gratuita)

- Python

- PyTorch, torchvision

- OpenCV

- NumPy, Pandas

- Matplotlib, Seaborn

- scikit-learn

---

## 🚀 Come Eseguire
1. Aprire il notebook direttamente in Google Colab.

2. Caricare il dataset come indicato sopra.

3. Eseguire tutte le celle del notebook per preprocessing, training e valutazione.

---

## 👤 Autore
Antonino Maenza
Progetto sviluppato durante la magistrale in Ingegneria Biomedica presso l’Università degli Studi di Palermo.
