🧠Carvana U-Net Project
Goal: Semantic segmentation of cars at pixel level.
Model: U-Net implemented from scratch using PyTorch.
Input: RGB car image [B, 3, H, W]
Output: Binary segmentation mask [B, 1, H, W]
0 → background
1 → car
Architecture:
Encoder → Bottleneck → Decoder
Skip connections between encoder and decoder.
Main files:
UNET_Carvana/
├── main.py
├── Unet.py
├── Unet_parts.py
├── requirements.txt
├── .gitignore
└── README.md
Training: BCEWithLogitsLoss + Adam.
Run:
python main.py
