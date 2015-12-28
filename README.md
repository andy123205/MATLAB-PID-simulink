# MATLAB-PID-simulink
simulation tutorial for PID controller

![pid](https://cloud.githubusercontent.com/assets/13445632/12025766/f3237312-adec-11e5-949a-95b9f43ffc0a.png)

MATLAB simulink教學

1.先開啟simulink 可以點選紅色圈圈裡的按鈕或是直接輸入simulink在command window裡面
![simulink1](https://cloud.githubusercontent.com/assets/13445632/12026388/fd0ce1f4-adf3-11e5-95a6-7261372712d6.png)

2.接著新增一個空白檔案
![simulink2](https://cloud.githubusercontent.com/assets/13445632/12026389/fd319602-adf3-11e5-8a25-b172064da21a.png)

3.搜尋你要的元件並且拖曳過來，這邊是步階響應(Step)
![simulink3](https://cloud.githubusercontent.com/assets/13445632/12026390/fd34764c-adf3-11e5-9005-1f67c05a31b8.png)

4.加法器(Sum)，等等會修改成減法器以滿足負回授的效果
![simulink4](https://cloud.githubusercontent.com/assets/13445632/12026391/fd51a802-adf3-11e5-908a-d4d09a62094f.png)

5.PIDcontroller
![simulink5](https://cloud.githubusercontent.com/assets/13445632/12026400/fdb8d59a-adf3-11e5-9bcd-04e608589ec4.png)

6.受控體(Plant)
![simulink6](https://cloud.githubusercontent.com/assets/13445632/12026392/fd55f0d8-adf3-11e5-8e9f-b0b435e798b6.png)

7.示波器(Scope)
![simulink7](https://cloud.githubusercontent.com/assets/13445632/12026394/fd58a850-adf3-11e5-9c43-94305cf2925d.png)

8.調整步階響應的參數
![simulink8](https://cloud.githubusercontent.com/assets/13445632/12026393/fd57753e-adf3-11e5-9f01-c4cb1d9c8f18.png)

9.將加法器修改成減法器
![simulink9](https://cloud.githubusercontent.com/assets/13445632/12026395/fd5b111c-adf3-11e5-9955-cd1dbeadcab1.png)

10.修改PID參數
![simulink10](https://cloud.githubusercontent.com/assets/13445632/12026396/fd775174-adf3-11e5-8b0a-651d5e1fa015.png)

11.修改受控體方程式
![simulink11](https://cloud.githubusercontent.com/assets/13445632/12026397/fd7c6f74-adf3-11e5-950c-e8550aab0655.png)

12.設訂模擬時間，並且觀看波形
![simulink12](https://cloud.githubusercontent.com/assets/13445632/12026398/fd7e772e-adf3-11e5-8ca7-def7ccffc170.png)

13.一次比較4種不同的PID參數並且比較波形，在此新用了一個元件Bus Creator
![simulink13](https://cloud.githubusercontent.com/assets/13445632/12026399/fd817122-adf3-11e5-9b81-b8dc8e142d1e.png)

14.對於受控體" 1/(s+1)(s+2) " 給予四個不同參數的PID 並且使用步階響應做為輸入，模擬波形圖
![simulink14](https://cloud.githubusercontent.com/assets/13445632/12026544/ca07f364-adf5-11e5-9476-d52374a78f0c.png)

四個波形分別為
1.黃色(yellow)P=1,I=0,D=0

2.紫色(purple)P=5,I=0,D=0

3.藍色(blue)  P=5,I=5,D=0

4.紅色(Red)   P=5,I=5,D=2

