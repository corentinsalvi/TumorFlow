# TumorFlow

Section 01 — Fondements mathématiques
L'EDP se décompose en deux termes : ∇·(D∇c) (diffusion spatiale des cellules) et ρc(1−c) (prolifération logistique). Chaque terme est expliqué biologiquement et mathématiquement, avec le modèle anisotrope de Swanson pour matière blanche/grise.


Section 02 — Schémas numériques
Comparaison des 3 schémas (Euler explicite, Euler implicite, Crank-Nicolson), avec les conditions CFL de stabilité et le calcul concret : pour BraTS en 3D, Euler explicite exige ~700 itérations là où Crank-Nicolson n'en nécessite que 10.


Section 03 — 6 étapes de code Python complet et commenté : chargement NIfTI → prétraitement → construction du Laplacien creux → simulation Crank-Nicolson → calibration MCMC → validation quantitative.


Section 04 — Simulateur interactif : clique sur le cerveau 2D pour poser un foyer tumoral, ajuste D et ρ en temps réel et observe la propagation. Le phénotype (invasif vs prolifératif) change selon le ratio D/ρ.


Section 05 — Table de validation avec les 6 métriques cibles (Dice ≥ 0.65, HD95 ≤ 8mm, etc.) comparées à l'état de l'art.