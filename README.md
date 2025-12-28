# 以 YOLOv12 為基礎之主動脈瓣物件偵測研究

本研究針對 AI CUP 2025「主動脈瓣物件偵測」競賽，探討 YOLOv12 在灰階 CT 影像上的表現。

## 資料集 (Dataset)

本專案使用之原始影像資料受限於檔案大小與競賽規範，未直接上傳至本儲存庫。請依以下說明取得資料：

1. **原始影像下載**: 請至 [AI CUP 2025 趨勢科技 T-Brain 競賽平台](https://tbrain.trendmicro.com.tw/Competitions/Details/42) 下載訓練集與測試集影像。
2. **標籤檔 (Labels)**: 
   - 訓練所需之 YOLO 格式標籤檔 (.txt) 已整理於本儲存庫之 `training_label.zip` (或 `labels/` 資料夾)。
   - 這些標籤檔對應 50 位病患中具主動脈瓣結構的 2,787 張影像。
3. **資料夾結構建議**:
   下載影像後，請確保路徑與 `aortic_valve_colab.yaml` 中設定一致：
   ```text
   /content/dataset/
   ├── images/       # 存放 .png 影像
   └── labels/       # 存放本倉庫提供的 .txt 標籤
