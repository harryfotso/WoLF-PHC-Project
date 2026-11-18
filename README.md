# WoLF-PHC Implementation & Extension (INFO-F409)

Projet de groupe (trois étudiants) visant à implémenter, analyser et étendre les algorithmes de renforcement multi-agents **PHC (Policy Hill-Climbing)** et **WoLF-PHC (Win or Learn Fast Policy Hill-Climbing)**, d'après les travaux de Bowling et Veloso (IJCAI 2001).

## 🚀 Objectifs du projet
1. **Implémentation :** Développement des agents PHC et WoLF-PHC appliqués au jeu à somme nulle *Matching Pennies*.
2. **Reproduction :** Simulation de l'auto-jeu (*self-play*) et reproduction de la comparaison de stabilité de la politique (Figure 2a de l'article de référence).
3. **Extension :** Évaluation de la vitesse d'adaptation des agents suite à un changement soudain du biais d'un adversaire fixe.

## 📂 Structure du dépôt
- `learners.py` : Logique des agents (mise à jour Q-learning, calcul de la politique moyenne, et sélection du pas selon le principe WoLF).
- `run_experiments.py` : Script principal pour exécuter les scénarios d'auto-jeu et de changement d'adversaire.
- `plot_results.py` : Génération des graphiques de trajectoire et de performance.
- `test_project.py` : Suite de tests unitaires et déterministes.
- `results/` : Dossier contenant les données sérialisées et les traces échantillonnées.

## 🛠️ Installation et Exécution
1. Cloner le dépôt et créer un environnement virtuel :
   ```bash
   python -m venv .venv
   # Sous Windows :
   .\.venv\Scripts\python -m pip install numpy matplotlib
   # Sous macOS / Linux :
   .venv/bin/python -m pip install numpy matplotlib
