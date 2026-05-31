# Application Android de Gestion et Analyse des Capteurs

## Présentation

Cette application Android développée en Java permet d’exploiter plusieurs capteurs présents sur un smartphone afin d’effectuer des mesures en temps réel, analyser les mouvements et visualiser différentes données physiques.

L’objectif principal du projet est d’étudier l’utilisation des capteurs Android ainsi que leur intégration dans une application mobile moderne.

---

# Objectifs du projet

L’application permet de :

- explorer les capteurs disponibles sur l’appareil ;
- récupérer des mesures en temps réel ;
- afficher graphiquement les données collectées ;
- détecter certains mouvements ;
- créer une boussole numérique ;
- compter les pas de l’utilisateur ;
- reconnaître des activités simples.

---

# Modules disponibles

## 1. Exploration des capteurs

Affichage des informations principales :

- identifiant du capteur
- nom
- fabricant
- version
- type
- précision
- consommation énergétique
- plage maximale
- fréquence minimale

---

## 2. Surveillance des capteurs environnementaux

Capteurs pris en charge :

- température
- humidité
- proximité
- champ magnétique

Fonctionnalités :

- affichage instantané des mesures
- mise à jour dynamique
- représentation graphique

---

## 3. Analyse du mouvement

Capteurs utilisés :

- accéléromètre
- gravité
- gyroscope

Informations affichées :

- valeurs X, Y et Z
- intensité du mouvement
- évolution temporelle

---

## 4. Boussole numérique

La direction est calculée à partir :

- du magnétomètre
- de l’accéléromètre

Affichage :

- angle de rotation
- orientation cardinale
- direction actuelle

---

## 5. Compteur de pas

L’application affiche :

- nombre total de pas
- nombre de pas pendant la session active

---

## 6. Reconnaissance d’activité

L’application réalise une détection simple :

- appareil immobile
- marche
- déplacement
- saut

---

# Architecture générale

```text
com.example.sensorsapp

├── MainActivity.java

├── fragments
│   ├── SensorsFragment.java
│   ├── GraphFragment.java
│   ├── MotionFragment.java
│   ├── CompassFragment.java
│   ├── StepFragment.java
│   └── ActivityFragment.java

├── helpers
│   └── SensorUtils.java

└── customviews
    └── ChartView.java
```

---

# Technologies utilisées

| Technologie | Utilisation |
|------------|------------|
| Java | Développement Android |
| Android Sensor API | Accès aux capteurs |
| SensorManager | Gestion des capteurs |
| SensorEventListener | Écoute des événements |
| CardView | Interface graphique |
| Navigation Drawer | Navigation |

---

# Installation

## Dépendance Gradle

```gradle
implementation 'androidx.cardview:cardview:1.0.0'
```

## Permission nécessaire

Ajouter :

```xml
<uses-permission android:name="android.permission.ACTIVITY_RECOGNITION"/>
```

---

# Interface utilisateur

L’application utilise :

- navigation latérale
- cartes interactives
- tableaux de bord
- graphes temps réel

---

# Résultats

Fonctionnalités validées :

- Lecture temps réel des capteurs
- Affichage graphique
- Détection du mouvement
- Navigation intuitive
- Interface moderne

---

# Auteur

AIT HMAD OUSSAMA 
