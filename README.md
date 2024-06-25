# Heat-Distribution-Simulation
這是一個熱擴散模擬器，用於模擬不同材料中的溫度變化，它基於有限差分方法，將空間離散化為網格，時間離散化為步驟，並使用熱擴散方程進行模擬。

## 功能和結構：
### 1.初始化和GUI設置：
  ##### a.使用Tkinter建立GUI，包括下拉選單來選擇材料類型。
  ##### b.可以選擇的材料包括鋼、銅、鋁和鐵，每種材料有不同的熱擴散率，影響溫度變化的速度和方式。
  ##### c.初始設置包括板的尺寸、空間步長、冷卻邊界溫度和加熱邊界溫度。
### 2.熱擴散模擬：
  ##### a.根據所選材料的熱擴散率，計算時間步長，以確保穩定的模擬。
  ##### b.初始溫度分佈設置為板的中央有一個加熱區域（以圓形表示），其餘區域為冷卻溫度。
  ##### c.使用有限差分法，計算每個時間步的溫度分佈。這包括將空間上的溫度變化（根據中央差分）和時間步長應用於溫度場。
### 3.動畫顯示：
  ##### a.使用Matplotlib的動畫功能顯示溫度分佈隨時間的演變。
  ##### b.每個動畫幀顯示一個時間步，並更新圖中的溫度圖像以反映新的溫度分佈。
  ##### c.每個時間步的標題顯示為“時間步數”，以及該時間步的溫度分佈情況。
### 4.交互性：
  ##### a.可以通過下拉選單隨時更改材料類型，重新計算溫度分佈並重新開始動畫。
  ##### b.GUI允許用戶直觀地查看不同材料如何影響溫度分佈的速率和模式。
