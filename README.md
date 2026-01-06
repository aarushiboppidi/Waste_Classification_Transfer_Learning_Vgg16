# TrashNet Image Classification

This project classifies waste images from the **TrashNet** dataset using:
- **VGG16 transfer learning** (frozen ImageNet)
- A **baseline CNN** trained for comparison with from scratch training

The models are trained in a **Google Colab** notebook using TensorFlow/Keras.

## Dataset
TrashNet dataset from Kaggle: (https://www.kaggle.com/datasets/feyzazkefe/trashnet)

## Models
**VGG16 Transfer Learning**
- Pretrained VGG16 (`include_top=False`)
- GlobalAveragePooling → Dense(256) → Dropout(0.5) → Softmax
- Adam optimizer (lr = 1e-4)
**Baseline CNN**
- 3 Conv blocks (32 → 64 → 128)
- Dense(128) + Dropout(0.5)

## How to Run
1. Upload dataset to Google Drive as `dataset-resized/`
2. Open the notebook in Google Colab
3. Run all the cells
