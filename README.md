### 目錄
1 背景介紹： ........................................................ 2

2 需求分析 .......................................................... 2

3 系統用例模型 ...................................................... 4

3.1 訂餐者用例圖 ................................................ 4

3.2 商家用例圖 .................................................. 4

3.3 店鋪管理員用例圖 ............................ 4

3.4 訂單管理員用例圖 ............................................ 5

3.5 系統管理員用例圖 ............................................ 6

4 系統靜態模型 ...................................................... 7

5 系統動態模型 ...................................................... 8

5. 系統時序圖 .................................................... 8
6. 
5.1 .1 訂餐者訂餐 ........................................... 8
   
5.1 .2 商家管理店鋪 ......................................... 9

5.1 .3 店鋪管理管理員管理店鋪 .............................. 1 0

5.1 .4 店鋪管理員建立客戶評價檔案 .......................... 1 1

5.1 .5 店鋪管理員建立商家監察檔案 .......................... 1 2

5.1 .6 訂單管理員管理訂單 .................................. 1 3

5.1 .7 系統管理員管理商家資訊 .............................. 1 4

5.1 .8 系統管理員管理訂餐者資訊 ............. 15

5.1 .9 系統管理員維護系統 .................................. 1 6


5.2 系統活動圖 ................................................. 1 7

5.3 系統狀態圖 ................................................. 1 7

6 系統部署模型 ..................................................... 1 8

6.1 系統構件圖 ................................................. 1 8

6.2 系統部署圖 ................................................. 1 8

7 總結 ....................................................
### 1 背景介紹
隨著網路技術的飛速發展， 人們的生活也越來越追求方便化。
經過觀察， 發
現整個大學城的學生對平常訂餐需求很大， 但他們訂餐的方式都是比較原始的電話訂餐。 
而各個餐飲店也是各自為戰， 自己接電話， 記錄訂單需求， 自己配送。這樣做效率很低， 利潤薄， 而且資訊不流暢。 
所以我決定為大學生提供一個平臺 網上訂餐系統。 在網上給申請的商家一個虛擬店面， 可以在上面掛上該商家的名稱， 飯菜的圖片和價格等資訊， 讓訂餐者可以方便地訂餐， 還可以對商家的餐飲進行評價， 由系統生成評價檔案以供其他人參考等， 而商家後期只負責做飯菜並安排人配送。
此外， 需要定期對商家進行衛生安全監察， 生成商家監察檔案，並以此為依據來決定商家的去留等。
###2 需求分析
大學生網上訂餐系統主要有以下幾方面需求：

1訂餐者

訂餐者首先需要註冊一個帳號用於系統登錄， 登錄後可以查看店鋪資訊， 並
選中某一店鋪後進入其餐飲資訊介面， 最終選中所需餐飲， 下訂單。 當然用餐後還可以對此餐飲進行評價。

2 商家

商家首先需要申請一個網上店鋪， 當申請通過後， 登錄到系統中， 可以核實
訂單並安排配送， 然後對本店的餐飲資訊進行更新。

3 訂單管理員

當訂餐者下訂單後， 訂單管理員需及時生成訂單， 如果訂餐者對訂單有所更
改時， 訂單管理員也要及時對資料進行更新。

4 店鋪管理員

當商家申請通過時， 店鋪管理員需要及時錄入店鋪資訊， 並為其設立店面、
建立客戶評價檔案、 商家監察檔案。 當商家增加、 修改、 刪除其餐飲資訊時， 店鋪管理員需及時對資料進行更新， 以便其他人訂餐。 
如果訂餐者對某餐飲店的某餐飲進行評價後， 店鋪管理員需及時更新評價檔案。

5 系統管理員

系統管理員主要完成對商家和訂餐者資訊的管理、 以及系統的維護。
3 系統用例模型
大學生網上訂餐系統的參與者有：
![image](https://github.com/james10292210/10924149-final/assets/149235583/e8e01570-8fa9-4e64-9f94-79a6cb293078)

### 3.1 訂餐者用例圖

訂餐者可以登錄系統， 登錄後可以訂餐， 訂餐過程包括選擇店鋪、 選擇餐飲、
下訂單以及到餐付款， 用餐後還可以對餐飲進行評價。

![image](https://github.com/james10292210/10924149-final/assets/149235583/6a3dfbb8-20c9-46e8-b17a-5ea38166c315)

### 3.2 商家用例圖

商家可以登錄系統， 登錄後需要對訂餐者的訂單進行核實並安排配送， 然後
更新店鋪有關餐飲資訊（增加、 刪除、 修改） 。

![image](https://github.com/james10292210/10924149-final/assets/149235583/fdc64ff1-ea3b-4b3e-b831-61840fdec60c)
### 3.3 店鋪管理員用例圖

店鋪管理員可以更新店鋪資訊（包括錄入新申請通過的商家、 修改、 刪除和
查詢店鋪資訊） ， 還要為每一個店鋪建立客戶評價檔案盒商家監察檔案。
### 3.4 訂單管理員用例圖

訂單管理員當訂餐者下訂單後要立即生成新訂單， 如更新（查詢、 修改、刪除） 

### 3.5 系統管理員用例圖

系統管理員可以登錄系統， 對商家和訂餐者的資訊進行管理（增加、 刪除、
修改、 查詢） ， 還有系統的維護。
![image](https://github.com/james10292210/10924149-final/assets/149235583/04e0175b-ca9a-4332-9ce2-df8f789fc60f)
### 4 系統靜態模型

由需求分析中知， 我們可以依據主要六個類物件： 訂餐者、 訂單管理員、 商
家、 店鋪管理員、 系統管理員、 訂單、 店鋪和餐飲創建完整的類圖 。
![image](https://github.com/james10292210/10924149-final/assets/149235583/d0ac0f24-a9ef-4c05-9b96-ce45dfec7b0d)
### 5.1 .1 訂餐者訂餐

（ 1） 訂餐者註冊一個系統登錄帳號；

（ 2） 在登錄介面輸入相應的用戶名和密碼進行身份驗證；

（ 3） 系統驗證後將驗證結果返回給用戶；

（ 4） 系統展示有關店鋪資訊；

（ 5） 訂餐者選擇店鋪；

（ 6） 系統展示該店鋪的有關餐飲資訊；

（ 7） 訂餐者流覽資訊並選擇所需餐飲；

（ 8） 訂餐者下訂單；

（ 9） 下訂單成功後， 系統更新餐飲資訊；

（ 1 0） 退出系統；

（ 1 1） 用餐後對餐飲進行評價。

![image](https://github.com/james10292210/10924149-final/assets/149235583/640e579f-b8fc-4dc5-8d6b-4c612a70a381)

根據訂餐者訂餐的時序圖可以創建如下協作圖：

![image](https://github.com/james10292210/10924149-final/assets/149235583/602f079f-ba09-4184-aaeb-1951484f7fef)

### 5.1 .2 商家管理店鋪 

（ 1） 商家申請一個網上虛擬店鋪；

（ 2） 申請成功後， 在登錄介面輸入自己的用戶名和密碼進行身份驗證；

（ 3） 系統進行驗證並將驗證結果返回給商家；

（ 4） 商家處理訂單；

（ 5） 更新店鋪相關餐飲資訊；

（ 6） 提交更新資料；

（ 7） 系統將提交的結果顯示給商家；

（ 8） 提交成功， 退出系統。

![image](https://github.com/james10292210/10924149-final/assets/149235583/dac6afee-4bd9-4934-a7cc-d16e84660472)

根據商家管理店鋪的時序圖可以創建如下協作圖：

![image](https://github.com/james10292210/10924149-final/assets/149235583/388853c2-0ef2-49c4-9708-313eb6cf6d87)

###　5.1 .3 店鋪管理員管理店鋪資訊

（ 1 ） 店鋪管理員登錄系統進入管理介面；

（ 2） 對店鋪的資訊進行更新；

（ 3） 提交更新資料；

（ 4） 系統將提交結果顯示給店鋪管理員；

（ 5） 提交成功， 退出系統。

![image](https://github.com/james10292210/10924149-final/assets/149235583/b1a2fe9e-8421-47c2-9c05-f601075d94af)

根據店鋪管理員管理店鋪資訊的時序圖可以創建如下協作圖：

![image](https://github.com/james10292210/10924149-final/assets/149235583/257f1afe-3c2d-4fe7-9f68-ea62d63717fa)

### 5.1 .4 店鋪管理員建立客戶評價檔案

（ 1 ） 店鋪管理員登錄到系統；

（ 2） 對訂餐者的評價進行核實並篩選；

（ 3） 生成最終的評價檔案；

（ 4） 系統將結果顯示給店鋪管理員；

（ 5） 退出系統。

![image](https://github.com/james10292210/10924149-final/assets/149235583/16d525e5-1adf-4393-b9a8-8059a3d28868)

根據店鋪管理員建立客戶評價檔案的時序圖可以創建如下協作圖：

![image](https://github.com/james10292210/10924149-final/assets/149235583/432e799b-1550-4c10-8f05-d8afbe7a2c75)

### 5.1 .5 店鋪管理員建立商家監察檔案

（ 1） 店鋪管理員登錄到系統；

（ 2） 錄入通過檢查得出的監察結果；

（ 3） 生成監察檔案；

（ 4） 系統將結果顯示給店鋪管理員；

（ 5） 退出系統。


![image](https://github.com/james10292210/10924149-final/assets/149235583/8e4a546c-0c98-4413-ab6a-5017981d4876)

根據店鋪管理員建立商家監察檔案的時序圖可以創建如下協作圖：

![image](https://github.com/james10292210/10924149-final/assets/149235583/a33061fc-5c5e-46ac-9c4d-3f452a5824fc)

### 5.1 .6 訂單管理員管理訂單

（ 1） 訂單管理員登錄到系統中；

（ 2） 管理訂單資訊；

（ 3） 提交更新資料；

（ 4） 系統將更新結果顯示給定單管理員；

（ 5） 提交成功， 退出系統。


 ![image](https://github.com/james10292210/10924149-final/assets/149235583/1ecfd77b-c9e0-4b90-a56c-22d3bc988774)
 

### 5.1 .7 系統管理員管理訂餐者資訊

（ 1） 系統管理員註冊一個自己的登錄帳號；

（ 2） 輸入用戶名和密碼進行身份驗證；

（ 3） 系統將驗證結果顯示結果返回給系統管理員；

（ 4） 系統管理員在訂餐者資訊管理介面對訂餐者資訊進行更新；

（ 5） 提交更新資料；

（ 6） 系統將提交結果返回；

（ 7） 提交成功， 退出系統。

![image](https://github.com/james10292210/10924149-final/assets/149235583/1dbc77e0-193d-45f1-8063-f50248307da0)

### 5.1 .8 系統管理員管理商家資訊 

（ 1） 系統管理員註冊一個自己的登錄帳號；

（ 2） 輸入用戶名和密碼進行身份驗證；

（ 3） 系統將驗證結果顯示結果返回給系統管理員；

（ 4） 系統管理員在商家資訊管理介面對商家資訊進行更新；

（ 5） 提交更新資料；

（ 6） 系統將提交結果返回；

（ 7） 提交成功， 退出系統。

![image](https://github.com/james10292210/10924149-final/assets/149235583/7579d986-e509-47be-a7c8-1d5d5e50a390)

### 5.1 .9 系統管理員維護系統

（ 1） 系統管理員註冊一個自己的登錄帳號；

（ 2） 輸入用戶名和密碼進行身份驗證；

（ 3） 系統將驗證結果顯示結果返回給系統管理員；

（ 4） 系統管理員在系統維護介面對系統進行維護；

（ 5） 提交維護操作；

（ 6） 系統將提交結果返回；

（ 7） 提交成功， 退出系統。

![image](https://github.com/james10292210/10924149-final/assets/149235583/a06bef07-7b37-4169-9587-6f4868a06dca)

### 5.2 系統活動圖 

根據大學生網上訂餐系統的整個活動過程， 創建了如下的系統活動圖：

![image](https://github.com/james10292210/10924149-final/assets/149235583/1090a3e6-0a54-473d-88a4-64eff80b46ac)

### 5.3 系統狀態圖

根據前面的分析和設計可以發現， 每個參與者在使用系統前都需要進行登
錄， 登錄之後就可以進行各自相應的操作， 操作完成後退出系統。 創建的系統狀
態圖如下：

![image](https://github.com/james10292210/10924149-final/assets/149235583/9534f757-363d-4351-afa7-757a4bdfffc0)

###6 系統部署圖

### 6.1 系統構件圖

網上訂餐系統的構件圖我們通過構件映射到系統的實現類中， 說明該構件物
理實現的邏輯類， 在本系統中， 我們可以對訂餐者類、 系統管理員類、 商家類、
店鋪管理員類、 訂單管理員類、 訂單類和餐飲類分別創建對應的構件進行映射。

![image](https://github.com/james10292210/10924149-final/assets/149235583/9812381f-2ee5-4955-a139-8c242e1a5a6f)

###6.2 系統部署圖 

網上訂餐系統的部署圖描繪的是系統節點上運行資源的安排。 包括四個節
點， 分別是： 用戶端流覽器、 HTTP伺服器、 資料庫伺服器和印表機。

![image](https://github.com/james10292210/10924149-final/assets/149235583/526a036c-0ecb-4648-9029-5d12bf95ea65)

### 7 總結

經過認真地分析我得出了系統的需求分析， 確定了系統的主要參與者以及各
自的主要活動。 
通過學習 UML建模的有關知識和 Rational Rose工具， 我親自動
手練習， 最終畫出了系統的系統用例模型（各自用例的用例圖） 、 系統靜態模型
（系統類圖） 、 系統的動態模型（系統時序圖、 系統活動圖和系統狀態圖） 以及
系統部署模型（系統構件圖和系統部署圖） 。
通過自己的親自動手操作， 使我進一步瞭解並掌握了 UML的建模過程和 Rational Rose工具的使用。 
同時， 我也發現了自己思考問題不全面等一系列不足， 促使自己不斷改正、 不斷進步。




























































 




