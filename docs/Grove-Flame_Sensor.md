---
name: Grove - Flame Sensor
category: Sensor
bzurl: https://seeedstudio.com/Grove-Flame-Sensor-p-1450.html
oldwikiname: Grove_-_Flame_Sensor
prodimagename: Flame_Sensor_01.jpg
bzprodimageurl: http://statics3.seeedstudio.com/images/product/Flame Sensor.jpg
surveyurl: https://www.research.net/r/Grove-Flame_Sensor
sku: 101020049
tags: grove_digital, io_5v, plat_duino, plat_linkit
---


![](https://raw.githubusercontent.com/SeeedDocument/Grove-Flame_Sensor/master/img/Flame_Sensor_01.jpg)

Bộ cảm biến ngọn lửa Grove có thể được sử dụng để phát hiện nguồn lửa hoặc các nguồn sáng khác có bước sóng trong phạm vi từ 760nm - 1100nm. Nó dựa trên cảm biến YG1006 là một phototransistor silicon NPN tốc độ cao và độ nhạy cao. Do epoxy đen, cảm biến rất nhạy cảm với bức xạ hồng ngoại. Trong trò chơi robot chữa cháy, cảm biến đóng vai trò rất quan trọng, nó có thể được sử dụng như mắt robot để tìm nguồn lửa.

[![](https://raw.githubusercontent.com/SeeedDocument/common/master/Get_One_Now_Banner.png)](http://www.seeedstudio.com/Grove-Flame-Sensor-p-1450.html)

## Đặc điểm

-   Giao diện Grove
-   Độ nhạy sáng cao
-   Thời gian đáp ứng nhanh
-   Dễ sử dụng
-   Độ nhạy được điều chỉnh

!!!Mẹo
    Thông tin chi tiết về các module Grove vui lòng tham khảo [Hệ thống Grove](http://wiki.seeedstudio.com/Grove_System/)

## Các thông số kỹ thuật


<table border="1" cellspacing="0" width="80%">
<tr>
<th scope="col">
Item
</th>
<th scope="col">
Min
</th>
<th scope="col">
Điển hình
</th>
<th scope="col">
Max
</th>
<th scope="col">
Đơn vị
</th>
</tr>
<tr align="center">
<th scope="row">
Điện áp
</th>
<td>
4.75
</td>
<td>
5.0
</td>
<td>
5.30
</td>
<td>
VDC
</td>
</tr>
<tr align="center">
<th scope="row">
Dòng điện
</th>
<td>
/
</td>
<td>
20
</td>
<td>
/
</td>
<td>
mA
</td>
</tr>
<tr align="center">
<th scope="row">
Phạm vi của băng thông quang phổ
</th>
<td>
760
</td>
<td>
940
</td>
<td>
1100
</td>
<td>
nm
</td>
</tr>
<tr align="center">
<th scope="row">
Phạm vi phát hiện
</th>
<td>
0
</td>
<td>
~
</td>
<td>
1
</td>
<td>
m
</td>
</tr>
<tr align="center">
<th scope="row">
Thời gian đáp ứng
</th>
<td colspan="3">
15
</td>
<td>
μS
</td>
</tr>
<tr align="center">
<th scope="row">
Nhiệt độ hoạt động
</th>
<td>
-25
</td>
<td>
~
</td>
<td>
85
</td>
<td>
℃
</td>
</tr>
</table>

## Các nền tảng được hỗ trợ


| Arduino                                                                                             | Raspberry Pi                                                                                             | BeagleBone                                                                                      | Wio                                                                                               | LinkIt ONE                                                                                         |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/arduino_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/raspberry_pi_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/bbg_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/wio_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/linkit_logo.jpg) |

!!!Chú ý
    Các nền tảng được đề cập ở trên được hỗ trợ như chỉ dẫn của phần mềm của module hoặc khả năng tương thích về mặt lý thuyết. Chúng tôi chỉ cung cấp thư viện phần mềm hoặc các ví dụ cho nền tảng Arduino trong hầu hết các trường hợp. Không thể cung cấp thư viện phần mềm / mã demo cho tất cả các nền tảng MCU. Do đó, người dùng phải viết thư viện phần mềm của riêng họ.

## Getting Started

Các mô-đun chủ yếu được sử dụng để phát hiện ánh sáng hồng ngoại. Nó xuất tín hiệu số 0 và 1 thông qua đầu ra Bộ so sánh. Giá trị đầu ra sẽ là 0 khi phát hiện thấy đèn hồng ngoại. Và độ nhạy được điều chỉnh bằng chiết áp chính xác.

### Đối với Arduino

#### Phần cứng
- **Bước 1.** Chuẩn bị những thứ dưới đây:

| Seeeduino V4.2 | Base Shield| Grove-Flame_Sensor |Grove - Red LED|
|--------------|-------------|-----------------|-----|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/seeeduino_v4.2.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/base_shield.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Flame_Sensor/raw/master/img/45d_small.jpg)|![enter image description](https://github.com/SeeedDocument/Grove-Red_LED/raw/master/img/Red%20LED_s.jpg)|
|[Get One Now](http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html)|[Get One Now](https://www.seeedstudio.com/Base-Shield-V2-p-1378.html)|[Get One Now](http://www.seeedstudio.com/Grove-Flame-Sensor-p-1450.html)|[Get One Now](https://www.seeedstudio.com/s/Grove-Red-LED-p-1142.html)|

- **Bước 2.** Kết nối Grove-Flame_Sensor tới cổng **D2** của Grove-Base Shield.
- **Bước 3.** Kết nối Grove - Red LED tới cổng **D3** của Grove-Base Shield.
- **Bước 4.** Cắm Grove - Base Shield vào Seeeduino.
- **Bước 5.** Kết nối Seeeduino tới PC qua một cáp USB.

<!--link-->
![with_ardu](https://github.com/SeeedDocument/Grove-Flame_Sensor/raw/master/img/with_ardu.jpg)

!!!Chú ý
Nếu chúng tôi không có Grove Base Shield, chúng tôi cũng có thể kết nối trực tiếp module này tới Seeeduino như dưới đây.

| Seeeduino       |  Grove-Flame_Sensor  |
|---------------|-------------------------|
| 5V           | Đỏ                     |
| GND           | Đen                   |
| Not Conencted | Trắng                   |
| D2            | Vàng                  |



| Seeeduino       |  Grove - Red LED |
|---------------|-------------------------|
| 5V           | Đỏ                     |
| GND           | Đen                   |
| Not Conencted | Trắng                   |
| D3            | Vàng                  |





#### Phần mềm


**Step 1.** Sao chép mã và flash nó vào bảng điều khiển.


Đây là code
```c
    /******************************************************************************/

#define FLAME_SENSOR 2 //connect SENSOR to digital pin2
#define LED 3 //connect Grove - LED to pin3

void setup()
{
    pinsInit();
}
void loop()
{
    if(isFlameDetected())
    turnOnLED();
    else turnOffLED();
}
    /********************************/
void pinsInit()
{
    pinMode(FLAME_SENSOR, INPUT);
    pinMode(LED,OUTPUT);
    digitalWrite(LED,LOW);
}
void turnOnLED()
{
    digitalWrite(LED,HIGH);
}
void turnOffLED()
{
    digitalWrite(LED,LOW);
}
boolean isFlameDetected()
{
    if(digitalRead(FLAME_SENSOR))
    return false;
    else return true;
}
```

**Bước 2.** Đèn LED sẽ sáng lên khi có đèn hồng ngoại. 

### Play with Codecraft

#### Đối với

**Bước 1.** Kết nối Grove - Flame Sensor tới cổng D2, và kết nối Grove - Red LED tới cổng D3 của Base Shield.

**Bước 2.** Cắm Base Shield vào Seeeduino/Arduino của bạn.

**Bước 3.** Kết nối Seeeduino/Arduino tới PC qua cáp USB.

#### Phần mềm

**Bước 1.** Mở [Codecraft](https://ide.chmakered.com/), thêm hỗ trợ Arduino và kéo một lệnh chính vào vùng làm việc.

!!!Chú ý
   Nếu đây là lần đầu tiên bạn sử dụng Codecraft, hãy xem thêm [Hướng dẫn sử dụng Codecraft bằng Arduino](http://wiki.seeedstudio.com/Guide_for_Codecraft_using_Arduino/).

**Bước 2.** Kéo các khối như hình dưới đây hoặc mở tệp cdc có thể được tải xuống ở cuối trang này.

![cc](https://raw.githubusercontent.com/SeeedDocument/Grove-Flame_Sensor/master/img/cc_Flame_Sensor.png)

Tải chương trình lên Arduino / Seeeduino của bạn.

!!!Kết quả
    Khi mã hoàn thành được tải lên, đèn LED sẽ sáng khi Cảm biến ngọn lửa phát hiện ngọn lửa.

### Đối với Raspberry Pi

#### Phần cứng

- **Bước 1.** Chuẩn bị những thứ dưới đây:


| Raspberry pi | GrovePi_Plus | Grove-Flame_Sensor |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/Grovepi%2B.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Flame_Sensor/raw/master/img/45d_small.jpg)|
|[Get One Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get One Now](https://www.seeedstudio.com/GrovePi%2B-p-2241.html)|[Get One Now](https://www.seeedstudio.com/Grove-Flame-Sensor-p-1450.html)|



- **Bước 2.** Cắm GrovePi_Plus vào Raspberry.
- **Step 3.** Kết nối Grove-Flame_Sensor  tới cổng **D2** của GrovePi_Plus.
- **Bước 4.** Kết nối Raspberry tới PC qua cáp USB.


![with_rpi](https://raw.githubusercontent.com/SeeedDocument/Grove-Flame_Sensor/master/img/with_rpi.jpg)

#### Phần mềm

- **Bước 1.** Theo dõi [Setting Software](https://www.dexterindustries.com/GrovePi/get-started-with-the-grovepi/setting-software/) để cài đặt môi trường phát triển.
- **Bước 2.** Git nhân bản kho lưu trữ Github.


```bash
cd ~
git clone https://github.com/DexterInd/GrovePi.git

```

-	**Bước 3.** Thực hiện các lệnh dưới đây để sử dụng cảm biến này


```bash
cd ~/GrovePi/Software/Python
python grove_flame_sensor.py
```


Đây là mã ví dụ:

```Python
#!/usr/bin/env python
#
# GrovePi Example for using the Grove Flame Sensor (http://www.seeedstudio.com/wiki/Grove_-_Flame_Sensor)
#
# The GrovePi connects the Raspberry Pi and Grove sensors.  You can learn more about GrovePi here:  http://www.dexterindustries.com/GrovePi
#
# Have a question about this example?  Ask on the forums here:  http://forum.dexterindustries.com/c/grovepi
#
'''
## License
The MIT License (MIT)
GrovePi for the Raspberry Pi: an open source platform for connecting Grove Sensors to the Raspberry Pi.
Copyright (C) 2017  Dexter Industries
Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:
The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
'''
import time
import grovepi

# Connect the Grove Flame Sensor to digital port D2
# SIG,NC,VCC,GND
flame_sensor = 2

grovepi.pinMode(flame_sensor,"INPUT")

while True:
    try:
        print(grovepi.digitalRead(flame_sensor))
        time.sleep(.5)

    except IOError:
        print ("Error")
```


## Tài liệu tham khảo

Cảm biến có thể phát hiện nguồn sáng có bước sóng nằm trong phạm vi từ 760nm - 1100nm. Hình dưới đây cho thấy độ nhạy phổ.
![](https://raw.githubusercontent.com/SeeedDocument/Grove-Flame_Sensor/master/img/Spectral_Sensitive.jpg)

## Nguồn

-  **[Eagle]** [Grove - Flame Sensor Eagle File](https://raw.githubusercontent.com/SeeedDocument/Grove-Flame_Sensor/master/res/Grove-Directional_Light_Sensor_Eagle_File.zip)
-  **[Library]** [Github repository for Grove_Flame_Sensor Library](https://github.com/Seeed-Studio/Grove_Flame_Sensor)
-  **[Datasheet]** [LM293D datasheet](https://raw.githubusercontent.com/SeeedDocument/Grove-Flame_Sensor/master/res/LM293D.pdf)
-  **[Codecraft]** [CDC File](https://raw.githubusercontent.com/SeeedDocument/Grove-Flame_Sensor/master/res/Grove_Flame_Sensor_CDC_File.zip)



## Hỗ trợ kỹ thuật
Vui lòng gửi bất kỳ vấn đề kỹ thuật vào [diễn đàn](http://forum.seeedstudio.com/) của chúng tôi.
<br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>