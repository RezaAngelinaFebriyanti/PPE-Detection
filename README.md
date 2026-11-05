# PPE Detection
Repository ini berisi implementasi dan pengujian model
YOLOv11s, SSD MobileNet, Faster R-CNN  untuk deteksi Alat Pelindung Diri
(APD) menggunakan CHVG Dataset.
## Struktur Repository
### YOLOv11
Berisi notebook untuk:
- Environment dan konfigurasi YOLOv11
- Implementasi dan training YOLOv11
- Pengujian model pada data test
### SSD-MobileNet
Berisi notebook untuk:
- Implementasi dan training SSD MobileNet
- Evaluasi model
- Pengujian model menggunakan data tes
## Requirements
YOLO :
- Ultralytics 8.4.157
- Python 3.10.12
- PyTorch 2.14.0+cpu

SSD MobileNet : 
- Python 3.10.12
- TensorFlow 2.15.1
- Protobuf 4.23.4
- libprotoc 27.3

Faster R-CNN :
- Python 3.10.6
- PyTorch 2.4.1
- Torchvision 0.19.1
- Torch-DirectML 0.2.5.dev240914 
- Numpy 2.2.6

## Dataset
- Data Training 70% (1.189 gambar)
- Data Validation 10% (170 gambar)
- Data Test 20% (340 gambar)
- 🔗 https://doi.org/10.6084/m9.figshare.19625166

## Hasil Pengujian Model

Pengujian dilakukan untuk membandingkan performa tiga model deteksi APD, yaitu Faster R-CNN, YOLOv11s, dan SSD MobileNet.

Evaluasi performa menggunakan metrik Precision, Recall, dan F1-Score.

### Hasil Data Evaluasi

| Model | Training | Precision | Recall | F1-Score |
|---|---|---:|---:|---:|
| Faster R-CNN | Epoch 10 | 85,52% | 89,27% | 87,35% |
| YOLOv11s | Epoch 20 | 84,30% | 79,40% | 81,78% |
| YOLOv11s | Epoch 30 | 86,20% | 81,10% | 83,57% |
| YOLOv11s | Epoch 40 | 86,20% | 82,70% | 84,41% |
| SSD MobileNet | 6.000 Steps | 39,06% | 27,58% | 32,33% |

### Hasil Data Test

| Model | Training | Precision | Recall | F1-Score |
|---|---|---:|---:|---:|
| Faster R-CNN | Epoch 10 | 86,15% | 89,22% | 87,66% |
| YOLOv11s | Epoch 40 | 91,65% | 81,89% | 86,49% |
| SSD MobileNet | 6.000 Steps | 36,86% | 24,28% | 29,27% |
