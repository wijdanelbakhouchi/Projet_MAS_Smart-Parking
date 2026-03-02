# Système Multi-Agents (MAS) pour Parking Intelligent

<p align="left">
  <img src="https://img.shields.io/badge/STATUT-PROJET%20ÉDUCATIF-0078D4?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/ARCHITECTURE-SYSTÈME%20MULTI--AGENTS-E87B1E?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/FRAMEWORK-JADE%20(JAVA)-606060?style=for-the-badge&logoColor=white" />
</p>

<p align="left">
  <img src="https://img.shields.io/badge/SIMULATION-PARKING%20TEMPS%20RÉEL-555555?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/ALGORITHME-OPTIMISATION-0078D4?style=for-the-badge&logoColor=white" />
</p>

> **Un système décentralisé intelligent conçu pour optimiser la gestion du stationnement urbain grâce à la coordination d'agents autonomes et à une prise de décision en temps réel.**
Ce projet compare les performances et revenus entre :

- gestion classique **FCFS – First Come First Served**
- gestion par **enchères dynamiques (Vickrey Auction)**

## Fonctionnalités

- **Simulation Multi-Agents (Mesa)**  
  Chaque voiture et chaque place de parking est un agent autonome.

- **Enchères de Vickrey**  
  Les voitures enchérissent pour les meilleures places selon leur budget.  
  Le gagnant paie **le prix de la deuxième meilleure offre**.

- **Visualisation en temps réel (React)**  
  Affichage de la grille, des mouvements et des indicateurs.

- **Tableau de bord KPI**  
  - taux d’occupation  
  - revenus générés  
  - distance totale parcourue

- **Architecture Client–Serveur**  
  - Backend : Python + FastAPI  
  - Frontend : React + Vite

## Tech Stack

### Backend (simulation)
- Python
- Mesa
- FastAPI
- Uvicorn

### Frontend (interface)
- React
- Vite
- Tailwind CSS
- Recharts
- lucide-react

## Structure du projet

```bash
smart-parking/
├── SmartParking_MAS/              # Logique Python
│   ├── agents.py                  # Définition des agents (Voitures, Places)
│   ├── model.py                   # Logique du modèle (grille, zones)
│   └── backend.py                 # API FastAPI
│
└── smart-parking-front/           # Interface React
    ├── src/
    │   └── SmartParkingClient.jsx # composant principal
    ├── package.json
    └── ...
```
## Installation et exécution

### Prérequis

- Python **3.8+**
- Node.js **16+**

### 1- Installation du Backend (Python)
```bash
cd parking-backend
pip install fastapi uvicorn mesa
uvicorn backend:app --reload
```
### 2- Installation du Frontend (React)
```bash
cd parking-frontend
npm install
npm install lucide-react recharts
npm run dev
```
## Utilisation

- ouvrir l’interface frontend
- vérifier l’état Backend Python Actif
- choisir mode FCFS ou Enchères
- régler le trafic
- démarrer / pause simulation

Légende :
- VIP ( Jaune )
- Handicap ( Blue )
- Standard ( Vert )

## Contribution
```bash
fork du projet
git checkout -b feature/NouvelleFeature
git commit -m "Add nouvelle feature"
git push origin feature/NouvelleFeature
```
ouvrir une Pull Request

## Licence

Projet académique — utilisation non libre.
contacter moi 




