# YOLOv8 Bottle Segmentation Interface

Interface OpenCV optimisée pour la détection et segmentation de bouteilles en temps réel.

## Structure du Projet

```
Double_Segementation_Water_Level/
├── models/
│   ├── best.pt                 # Modèle entraîné (segmentation bouteilles)
│   └── yolov8m-seg.pt          # Modèle de base YOLOv8m
├── training_results/
│   ├── results.png             # Courbes d'entraînement
│   ├── results.csv             # Métriques détaillées
│   ├── confusion_matrix_normalized.png
│   └── args.yaml               # Configuration d'entraînement
├── interface_opencv.py         # Interface principale
└── README.md                   # Documentation
```

## Utilisation

1. **Ouvrir le fichier** `interface_opencv.py` dans VS Code
2. **Cliquer sur la flèche "Run"** en haut à droite
3. **L'interface s'ouvre automatiquement** avec la webcam

## Contrôles

- **Q ou ESC** : Quitter l'application
- **SPACE** : Pause/Reprendre la détection
- **S** : Prendre un screenshot

## Performances

- **FPS** : ~40 FPS
- **Temps d'inférence** : ~24ms
- **GPU** : CUDA activé
- **Résolution** : 640x832

## Modèles

| Fichier | Description |
|---------|-------------|
| `models/best.pt` | Modèle entraîné pour la segmentation de bouteilles |
| `models/yolov8m-seg.pt` | Modèle de base YOLOv8 medium |

---
*Interface prête à l'emploi - Cliquez simplement sur Run !*