
# objectdetectionDemo
 使用客製化資料將Yolov8模型部署在手機上
 
(一)物體辨識 App 實作
我這幾天想從資料的收集到模型部署到程式裡的整個流程都基本跑過一遍，所以會這幾天大概會根據下列這幾個步驟實現一個能在 iOS 和 Android 上辨識一般物體(加上我自己的手套)的App。

以下是大致的流程，實際上應該還有很多的事要做:

1. 資料準備
收集和整理客製化資料集。
對資料集進行標註，標記出物體的邊界框和類別。

2. 模型訓練
 
 YOLOv8：
 
 下載YOLOv8的官方代碼和預訓練模型。
 修改配置文件，以適應客製化資料集。
 在GPU環境下，使用您的資料集訓練和評估YOLOv8模型。
 
3. 模型轉換

 將訓練好的模型轉換為適合移動端部署的格式，例如ONNX、TFLite或Core ML。
 
4. 移動端部署

 Android：
 
 如果使用TFLite格式，可以使用TensorFlow Lite Android Library進行部署。
 如果使用ONNX格式，可以使用ONNX Runtime Mobile進行部署。
 
 iOS：
 
 如果使用Core ML格式，可以使用Core ML framework進行部署。
 如果使用ONNX格式，可以使用ONNX Runtime Mobile進行部署。

5. 應用程式開發
使用移動應用開發框架（如React Native、Flutter、Swift、Kotlin等）開發app。
集成物體檢測模型，並實現相應的功能和界面。

6. 測試和優化
在不同的手機和環境下測試應用程式的性能和準確性。
根據測試結果進行模型和應用程式的優化。
性能考慮：移動端的計算資源有限，可能需要對模型進行優化，以達到實時性能。

7. 發布和更新
將完成的應用程式發布到Google Play Store或Apple App Store。
根據用戶反饋和需求進行後續的更新和優化。
隱私和安全：確保應用程式符合資料保護法規，保護用戶隱私。



