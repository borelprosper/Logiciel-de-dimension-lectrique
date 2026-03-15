# ⚡ NFC-DIM

**Application de dimensionnement électrique conforme à la norme NF C 15-100**

---

## 📖 Description

**NFC-DIM** est une application de bureau développée en **Python avec Tkinter** permettant de réaliser le **dimensionnement des installations électriques basse tension** conformément à la **norme NF C 15-100**.

Ce logiciel a été conçu pour aider les **techniciens, ingénieurs et étudiants en génie électrique** à effectuer rapidement les calculs nécessaires lors de la conception d'une installation électrique.

L'application automatise plusieurs opérations importantes :

- calcul du **courant nominal**
- dimensionnement des **sections de câbles**
- choix des **disjoncteurs**
- vérification de la **chute de tension**
- réalisation du **bilan de puissance**

Elle permet également de **générer des rapports techniques PDF** exploitables dans un dossier d'étude électrique.

---

# 🚀 Fonctionnalités

## 📁 Gestion des projets

- Création d’un **nouveau projet**
- Ouverture d’un **projet existant**
- Sauvegarde des données au **format JSON**

---

## 🔌 Carnet de câbles

Saisie des informations :

- Désignation de l’équipement
- Tension
- Puissance
- Longueur du câble
- Type de câble (**Cuivre / Aluminium**)
- Facteur de puissance (**cos φ**)
- Type d’équipement

Calcul automatique :

- Courant nominal
- Section normalisée du câble
- Calibre du disjoncteur
- Chute de tension

Limites de chute de tension respectées :

- **3 % pour l’éclairage**
- **5 % pour les autres usages**

---

## ⚡ Bilan de puissance

Saisie des charges :

- Nom de l’équipement
- Puissance unitaire
- Quantité
- Tension d’alimentation
- Fréquence
- Facteur de simultanéité
- Type de charge
- Source d’alimentation

Calcul automatique :

- Puissance installée
- Puissance demandée
- Puissance appelée
- Courant total
- Dimensionnement du **disjoncteur principal**
- Estimation de la **puissance du groupe électrogène**

---

## 📄 Génération de rapports PDF

L’application permet de générer deux documents :

### 📘 Carnet de dimensionnement des sections câblées

Contenant :

- désignation
- type de câble
- tension
- courant
- disjoncteur
- section
- chute de tension

### 📗 Bilan de puissance

Contenant :

- tableau des charges
- résultats de dimensionnement

Les rapports incluent :

- un **en-tête technique**
- les **informations du projet**
- un **logo**
- une **date d’impression automatique**

---

# 🛠 Technologies utilisées

- **Python**
- **Tkinter** (interface graphique)
- **ReportLab** (génération PDF)
- **Pillow** (gestion des images)
- **PyInstaller** (création d’un exécutable `.exe` monofichier)

---

# ⚙️ Compilation

Pour générer l'exécutable Windows :

```bash
pyinstaller nfcdim.spec
