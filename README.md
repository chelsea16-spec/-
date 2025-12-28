# 以 YOLOv12 為基礎之主動脈瓣物件偵測研究

本研究針對 AI CUP 2025「主動脈瓣物件偵測」競賽，探討 YOLOv12 在灰階 CT 影像上的表現。

## 實驗設定
- **模型版本**: YOLOv12-N
- **資料分配**: 訓練集與驗證集比例 45:5
- **資料增強**: 採用 RandAugment 與 Random Erasing (0.4)
- **環境**: Google Colab (NVIDIA T4 GPU)

## 效能表現
- **Public Score**: 0.9384 (IoU=0.55, Conf=0.2)
- **Private Score**: 0.9409 (IoU=0.6, Conf=0.05)

