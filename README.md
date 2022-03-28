# PlatformIO_Installation_Guide

## 一、下載安裝VSC
### Step 1. 下載 Visual Studio Code (VSC)
下載網址 https://code.visualstudio.com/

![1](https://user-images.githubusercontent.com/96014379/160340055-64dd95fc-2cb9-49b0-a621-4199330ad9a6.png)

記得其他內的選項全部都要打勾
![2](https://user-images.githubusercontent.com/96014379/160340739-af78be16-45ce-4656-8c2e-e1d5a4fa2a9e.png)

安裝畫面
![3](https://user-images.githubusercontent.com/96014379/160340811-0e8113e9-64ff-462f-afeb-91c64376a010.png)

### Step 2. 第一次啟動時，可能會推薦安裝中文語言包；或進入延伸模組，搜尋 chinese 手動安裝繁體中文語言包。

![4](https://user-images.githubusercontent.com/96014379/160340955-fd8c5dcd-820a-465f-90aa-98ecab96b494.png)

## 二、加入 PlatformIO
### Step 1. 進入延伸模組，搜尋 "PlatformIO" 手動安裝

![5](https://user-images.githubusercontent.com/96014379/160341108-7b136a10-14b9-43d8-bbfb-15b7084cb85e.png)

### Step 2. 安裝完後重新啟動 VSC，左側會出現 PlatformIO 的圖示。

![6](https://user-images.githubusercontent.com/96014379/160341179-1de648c4-535b-4add-a23d-a5e7193f39b3.png)

## 三、安裝Platform
開發版除了預設的板子(nano,uno)可以直接上傳程式，其他都要先安裝Platform(類似開發版環境)
Teensy->裝Teensy
ESP32->裝Espressif32
ESP8266->裝Espressif 8266
詳細安裝步驟參考下文

以ESP32為例:
### Step 1. 進入platformIO >> PIO HOME >> Open >> Platform

![7](https://user-images.githubusercontent.com/96014379/160341362-f076551b-f678-47d2-b053-ede283665a90.png)

### Step 2. 選擇Embedded，搜尋”espressif”，進入Espressif32。

![8](https://user-images.githubusercontent.com/96014379/160341431-cc72c25c-9be8-40d6-b209-bb20e12809cc.png)

### Step 3. 安裝，需耗時 5~10 分鐘。
![9](https://user-images.githubusercontent.com/96014379/160341472-4ce4dc50-dcaf-415f-9304-6b997b499d44.png)

### Step 4. 安裝完成。

![10](https://user-images.githubusercontent.com/96014379/160341596-02d0bebb-8ec1-4f81-a1ff-bb59e9872141.png)

### Step 5. 同樣方法搜尋 "teensy"，安裝teensy開發環境，Platform >> Installed可以看到安裝的環境 。ESP8266同理。
![11](https://user-images.githubusercontent.com/96014379/160341685-aa665738-46d3-4ede-99f7-e46bd9e2ede8.png)

## 四、開新專案
裝好要燒入板子的Platform，就可以開新專案準備燒入程式

### Step 1. 進入platformIO >> PIO HOME >> Projects，"Creat New Project"

![12](https://user-images.githubusercontent.com/96014379/160341810-91317fa0-633b-41fe-865b-d63782089a1c.png)

### Step 2. 建立專案名稱，及選擇MCU，esp32選擇”NodeMCU-32S”，可直接輸入；儲存位置預設為: (D:\Users\IEC5892M\Documents\PlatformIO\Projects)底下。

![13](https://user-images.githubusercontent.com/96014379/160341889-5cd682db-e25e-47c4-924d-52cacfe5eb5c.png)

補充:
Teensy:Board選對應的4.0選40，3.2選31
ESP32 : Board選NodeMCU-32S
ESP8266:Board 選Espressif Generic ESP8266 ESP-001 1M

取消預設可指定儲存位置。
![14](https://user-images.githubusercontent.com/96014379/160341955-bc70542d-e640-4c5c-bc5e-db120bd9f0ca.png)

### Step 3. 按下 finish 建構專案，重新啟動VSC後建專案可能會花比較多時間 3~10 min都有可能。

