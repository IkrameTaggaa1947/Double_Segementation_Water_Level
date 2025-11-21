# 🍶 YOLOv8 Bottle Segmentation Interface

Interface OpenCV optimisée pour la détection et segmentation de bouteilles en temps réel.

## Structure du Projet

```
3 segmentations.v4i.yolov8/
├── .vscode/                    # Configuration VS Code
│   ├── launch.json            # Configuration de débogage
│   └── settings.json          # Paramètres Python
├── runs/
│   └── segment/
│       └── bottle_final_quality/
│           └── weights/
│               └── best.pt    #  Modèle principal optimisé
├── interface_opencv.py         #  Interface principale
├── yolov8m-seg.pt             #  Modèle de fallback
└── README.md                  #  Documentation
```

##  Utilisation

1. **Ouvrir le fichier** `interface_opencv.py` dans VS Code
2. **Cliquer sur la flèche "Run" ** en haut à droite
3. **L'interface s'ouvre automatiquement** avec la webcam

## 🎮 Contrôles

- **Q ou ESC** : Quitter l'application
- **SPACE** : Pause/Reprendre la détection
- **S** : Prendre un screenshot

##  Performances

- **FPS** : ~40 FPS
- **Temps d'inférence** : ~24ms
- **GPU** : CUDA activé
- **Résolution** : 640x832

##  Fichiers Supprimés

Les fichiers suivants ont été supprimés car ils ne sont pas nécessaires au fonctionnement de l'interface :

### 📄 Scripts et Fichiers de Configuration
- `interface_auto.py` - Version alternative
- `interface_opencv_fixed.py` - Version de backup
- `quick_test.py` - Script de test
- `train_model.py` - Script d'entraînement
- `data.yaml`, `dataset.yaml` - Configuration d'entraînement
- `README.dataset.txt`, `README.roboflow.txt` - Documentation d'entraînement

###  Modèles Non Utilisés
- `yolov8n.pt` - Modèle nano (non utilisé)
- `yolov8s-seg.pt` - Modèle small (non utilisé)
- Tous les modèles d'époque (`epoch*.pt`, `last.pt`)

###  Dossiers d'Entraînement
- `test/`, `train/`, `valid/` - Datasets d'entraînement
- `outputs/` - Sorties d'entraînement
- `yolov8_pipeline/` - Pipeline d'entraînement
- Anciens runs d'entraînement (7 dossiers supprimés)

##  Configuration Technique

- **Python** : Utilise l'environnement virtuel configuré
- **Répertoire de travail** : Se place automatiquement dans le bon dossier
- **VS Code** : Configuration optimisée pour le debug et l'exécution

## Espace Disque Économisé

Le nettoyage a permis de supprimer plusieurs GB de fichiers non nécessaires tout en conservant la pleine fonctionnalité de l'interface.

---

*Interface prête à l'emploi - Cliquez simplement sur Run ! 🚀*
