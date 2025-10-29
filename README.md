<div align="center">
  <br />
  <img src="https://www.simplon.ma/images/Simplon_Maghreb_Rouge.png" alt="Simplon Maghreb Logo" width="300"/>
  <br /><br />

  <div>
    <img src="https://img.shields.io/badge/-Python-black?style=for-the-badge&logo=python&logoColor=white&color=3776AB" />
    <img src="https://img.shields.io/badge/-TensorFlow-black?style=for-the-badge&logo=tensorflow&logoColor=white&color=FF6F00" />
    <img src="https://img.shields.io/badge/-Keras-black?style=for-the-badge&logo=keras&logoColor=white&color=D00000" />
    <img src="https://img.shields.io/badge/-NumPy-black?style=for-the-badge&logo=numpy&logoColor=white&color=013243" />
    <img src="https://img.shields.io/badge/-Matplotlib-black?style=for-the-badge&logo=plotly&logoColor=white&color=11557C" />
    <img src="https://img.shields.io/badge/-Pandas-black?style=for-the-badge&logo=pandas&logoColor=white&color=150458" />
    <img src="https://img.shields.io/badge/-Google_Colab-black?style=for-the-badge&logo=googlecolab&logoColor=white&color=F9AB00" />
    <img src="https://img.shields.io/badge/-Jira-black?style=for-the-badge&logo=jira&logoColor=white&color=0052CC" />
  </div>

  <h1>🧠 Projet Deep Learning – Classification d’Images (Fashion MNIST)</h1>
  <p><strong>Projet IA</strong> – Simplon Maghreb</p>
</div>

---

## 🧩 1. Introduction

L’objectif de ce projet est de concevoir un **réseau neuronal dense minimaliste (DNN)** capable de classifier les images du dataset **Fashion MNIST** (28×28 pixels, 10 classes d’articles : t-shirts, chaussures, sacs, etc.).  
Le but est de **valider le pipeline complet** d’un projet de Deep Learning, de la **préparation des données** jusqu’à **l’évaluation du modèle**.

---

## ⚙️ 2. Modèle Utilisé

Le modèle est construit à l’aide de **TensorFlow/Keras** avec l’architecture suivante :

Flatten(input_shape=(28, 28))
Dense(128, activation='relu')
Dense(10, activation='softmax')


- **Optimiseur** : Adam  
- **Loss function** : sparse_categorical_crossentropy  
- **Métrique** : accuracy  
- **Callbacks** : EarlyStopping (basé sur val_loss)  

Les images ont été **normalisées (valeurs /255)** afin d’accélérer la convergence du modèle.

---

## 📈 3. Résultats Obtenus

| Jeu de Données | Accuracy | Loss |
|-----------------|-----------|------|
| **Test Set** | **0.8831** | **0.3427** |

### 🔍 Analyse des Résultats

- Le modèle atteint une **précision de 88.3 %**, dépassant l’objectif fixé (>80%).  
- Les performances sont cohérentes avec les limites d’un DNN simple, sans convolution.  
- Les erreurs de classification proviennent principalement des classes visuellement proches (ex. : *T-shirt* vs *Pullover*).

---


---

<div align="center">
  <p>👨‍💻 Projet réalisé par <strong><a href="https://github.com/OclaZ">OclaZ</a></strong> | Simplon Maghreb</p>

</div>

