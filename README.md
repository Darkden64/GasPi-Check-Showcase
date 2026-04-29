C'est rageant, GitHub a littéralement "mangé" ton tableau au lieu de l'afficher. C'est parce que le formatage Markdown est parfois trop sensible aux espaces.

Regarde ta capture : le texte est là, mais les images ont disparu. On va régler ça avec un code HTML ultra-simple. Le HTML, GitHub ne peut pas le rater, il est obligé de l'afficher correctement.

Efface tout à nouveau et colle ce bloc exact :
HTML

# GasPi-Check V9.5 — The Enviro-Tech Impact Engine 🌍

<table width="100%">
  <tr>
    <td align="center" width="33%"><b>Dashboard</b><br><img src="dashboard-alerte.png" width="200"></td>
    <td align="center" width="33%"><b>Impact Global</b><br><img src="stats-donut.png" width="200"></td>
    <td align="center" width="33%"><b>Frigo Familial</b><br><img src="scan-barcode.png" width="200"></td>
  </tr>
</table>

> "Turning food waste data into actionable climate positive assets." Une plateforme Enviro-Tech alliant gestion intelligente, gamification (Zen-Eco) et Big Data RSE.

## 🏗 Architecture Standard
* **Frontend** : React Native / Expo / TypeScript (Strong Typing).
* **Cloud Sync** : Firebase Firestore Real-time (Family Sync jusqu'à 6 membres).
* **Local-First** : Architecture hybride AsyncStorage/Cloud pour une performance offline-first.

## 🎮 Gamification & Behavioral Science
* **Économie Hardcore** : Système punitif/récompensant (+50/-200 XP) pour un changement de comportement réel.
* **Grades Zen-Eco** : 10 paliers de progression avec cartes de pouvoirs stratégiques (Turbo XP, Reset).
* **Statistiques** : Bandeau blanc arrondi avec trois colonnes (Gain XP, Perte XP, Efficacité) et vue hebdomadaire par défaut.

## 🛡 Privacy & RGPD Compliance
* **Kill Switch (V9.5)** : Suppression instantanée et totale des données (Cloud & Local).
* **Anonymisation** : IDs rotatifs et Data Minimization (Zéro tracking nominatif).

## 📊 Impact RSE
* **Barcode Analytics V2** : Insights sur le gaspillage post-achat par EAN.
* **Équivalences CO2** : Traduction de l'impact en mesures concrètes (Vols NY, Arbres).
* **Sentinelle** : Suppression automatique de la corbeille le dimanche à 23h59.
