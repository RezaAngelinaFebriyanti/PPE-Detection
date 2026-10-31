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
## Dataset
- Data Training 70% (1.189 gambar)
- Data Validation 10% (170 gambar)
- Data Test 20% (340 gambar)
- 🔗 https://doi.org/10.6084/m9.figshare.19625166
