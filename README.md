# GasPi-Check-Showcase
 Présentation de l'application GasPi-Check (V6.5) 
**L'assistant intelligent qui transforme le gaspillage alimentaire en impact écologique positif.**

GasPi-Check n'est pas une simple liste de courses. C'est un écosystème complet de gestion alimentaire utilisant la gamification "Hardcore" et des algorithmes écologiques pour réduire radicalement votre empreinte carbone.

## 🚀 Fonctionnalités Clés (V6.5)

### 1. Système de Statistiques & Impact (Dashboard Blanc)
* **Sélecteur de Période Dynamique** : Visualisation des performances par vue **Journalière (par défaut)**, **Hebdomadaire**, **Mensuelle** et **Annuelle**.
* **Bandeau de Performance XP** : Affichage en trois colonnes du gain, de la perte d'XP et du score d'efficacité avec message de rétroaction dynamique selon vos résultats.
* **Analyse CO2 Hybride** : Calcul de l'impact carbone via l'API **Open Food Facts** (Agribalyse) avec un système de repli (fallback) intelligent par catégorie (Viandes, Laitiers, Fruits & Légumes, etc.).

### 2. Gamification "Hardcore Mode"
* **Règles Strictes** : 0 XP à l'ajout (l'effort commence à la consommation +50xp ou +20xp selon la fraîcheur de l'aliment), **-200 XP** pour le gâchis volontaire (bouton Jeter) et **-100 XP** pour les produits périmés.
* **Zen-Eco Grades** : Une progression à travers 10 grades narratifs (de "Novice des stocks" à "Légionnaire Éternel de la Terre") avec des défis spécifiques par palier.
* **Eco-Legacy 2026** : Un moteur de quêtes mensuelles avec un hub "Gaming" permettant de débloquer des cartes d'avantages et des trophées.

### 3. Gestion Intelligente du Stock
* **Scanner Hybride** : Ajout rapide via scan de code-barres ou saisie manuelle avec catégorisation automatique.
* **Sentinelle de Péremption** : Alertes Push locales configurées à **J-1** et **J-0 (09h00)** pour garantir qu'aucun aliment ne soit oublié.

### 4. Expérience Utilisateur (UX)
* **Design Bio-Design** : Interface épurée avec accordéons rétractables pour "Ma Nourriture" et "Statistiques".
* **Sanctuaire du Frigo** : Système de *Streak* (flamme 🔥) récompensant les jours consécutifs sans gâchis avec des multiplicateurs d'XP.

### 5. 📸 Aperçu de l'Application
<img src="https://github.com/Darkden64/GasPi-Check-Showcase/blob/main/dashboard-alerte.png?raw=true" width="300" alt="Capture d'écran de GasPi-Check" />
<img src="https://github.com/Darkden64/GasPi-Check-Showcase/blob/main/scan-barcode.png?raw=true" width="300" alt="Capture d'écran de GasPi-Check" />
<img src="https://github.com/Darkden64/GasPi-Check-Showcase/blob/main/stats-donut.png?raw=true" width="300" alt="Capture d'écran de GasPi-Check" />

## 🛠 Stack Technique
* **Frontend** : React Native (Expo) & TypeScript.
* **Données** : Open Food Facts API & Agribalyse.
* **Graphiques** : Moteur hybride SVG (Web) et Native Charts.
* **Persistance** : AsyncStorage avec moteur de synchronisation temporelle (Time Travel Debugger).

## 👨‍💻 Créateur
**Darkden64** — Conception & Développement intégral — [Profil GitHub](https://github.com/Darkden64)

---
*Développé avec passion pour sauver la planète, un yaourt à la fois. 🌿*
