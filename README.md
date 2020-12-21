# Python-tello-face-tracker
這是一份copy paste的學生實作，內容含有非典型程式寫法與無法處理的報錯內容，以及可能存在預期外的錯誤



## 事前準備
下載這個github

下載DjiTelloPy 所需的插件集合
pip install https://github.com/damiafuentes/DJITelloPy/archive/master.zip

補充下載需要的插件
pip install imutils

至指定路徑啟動程式
python tello_face.py

## 介面
左上顯示畫面中心與偵測到的臉部中心XY軸距離差
畫面中則標示出兩者
Tello飛行器將逐漸修正至兩點重疊

## 預期中的錯誤
1.程式中沒有完整的關閉控制項目，當使用Esc停止程式仍然需要等候15秒直到超時錯誤回傳才會完整停止
2.開始執行時tello視訊與影像解碼器關鍵幀不同步，必然會跳出大量H.264警告，無視即可

## 預期外的錯誤
如果我知道就不叫預期外了Q
