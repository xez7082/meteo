# 🌤️ Météo HA - Glassmorphism Dashboard

Une interface météo interactive et ultra-moderne pour **Home Assistant**, utilisant les principes du **Glassmorphism**. Cette carte offre un rendu visuel dynamique en temps réel avec des effets de particules (pluie, neige, étoiles) basés sur l'état de vos capteurs.

---

## ✨ Points forts

* **Design "Glass"** : Effets de flou d'arrière-plan (`backdrop-filter`), bordures translucides et ombres portées diffuses.
* **Moteur de Rendu Canvas** : Animations fluides gérées par un script léger pour simuler la météo (soleil, orage, brouillard, etc.).
* **Adaptation Dynamique** : Les couleurs des bordures et des badges changent selon l'heure (lever/coucher de soleil) et les conditions.
* **Module Pollen & Air** : Visualisation claire des concentrations et des niveaux de risque par type de pollen.
* **Zéro Code YAML complexe** : La configuration des entités se fait directement via l'interface graphique intégrée à la carte.

---

## 🚀 Installation

### 1. Préparation du fichier
Enregistrez le code HTML complet dans un fichier nommé `meteo-glass.html` et placez-le dans votre dossier `/config/www/` de Home Assistant.

### 2. Configuration dans Lovelace
Ajoutez une carte de type **Webpage** (Page Web) à votre tableau de bord :
```yaml
type: iframe
url: /local/meteo-glass.html
aspect_ratio: 75%
