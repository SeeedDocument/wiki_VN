---
name: Grove - Relay
category: Actuator
bzurl: https://www.seeedstudio.com/Grove-Relay-p-769.html
oldwikiname:
prodimagename: Twig-Relay.jpg
surveyurl: https://www.surveymonkey.com/r/Grove_Relay
sku: 103020005
tags: io_3v3, io_5v, plat_duino, plat_linkit, plat_bbg, plat_pi,plat_wio
---


<p style=":center"><img src="https://raw.githubusercontent.com/SeeedDocument/Grove-Relay/master/img/Twig-Relay.jpg" /></p>




Module Grove-Relay là một công tắc kỹ thuật số thường mở. Thông qua nó, bạn có thể điều khiển mạch điện áp cao với điện áp thấp, giả sử 5V trên bộ điều khiển. Có một đèn LED chỉ báo trên bảng, đèn sẽ sáng lên khi các thiết bị đầu cuối được điều khiển đóng lại.
<iframe width="800" height="450" src="https://www.youtube.com/embed/MwLEawbP0ZU" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<p style=":center"><a href="https://www.seeedstudio.com/Grove-Relay-p-769.html" target="_blank"><img src="https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/300px-Get_One_Now_Banner-ragular.png" /></a></p>


## Phiên bản


| Tham số     | V1.1     |V1.2     |
| :------------- | :------------- |:------------- |
| Ngày phát hành     | 27/01/2013       |09/06/2014|
|Điện áp hoạt động|5V|3.3V~5V|
|Dòng hoạt động|60mA|100mA|
|Vòng đời rơle|100,000 Cycle|100,000 Cycle|
|Điện áp chuyển mạch tối đa|250VAC/30VDC|250VAC/30VDC|
|Dòng điện chuyển mạch tối đa|5A|5A|

!!!Mẹo
    Thông tin chi tiết về các module Grove vui lòng tham khảo [Hệ thống Grove](http://wiki.seeedstudio.com/Grove_System/)

## Các nền tảng được hỗ trợ


| Arduino                                                                                             | Raspberry Pi                                                                                             | BeagleBone                                                                                      | Wio                                                                                               | LinkIt ONE                                                                                         |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/arduino_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/raspberry_pi_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/bbg_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/wio_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/linkit_logo.jpg) |

!!!Chú ý
    Các nền tảng được đề cập ở trên được hỗ trợ như chỉ dẫn của phần mềm của module hoặc khả năng tương thích về mặt lý thuyết. Chúng tôi chỉ cung cấp thư viện phần mềm hoặc các ví dụ cho nền tảng Arduino trong hầu hết các trường hợp. Không thể cung cấp thư viện phần mềm / mã demo cho tất cả các nền tảng MCU. Do đó, người dùng phải viết thư viện phần mềm của riêng họ.



## Getting Started

### Đối với Arduino


!!!Chú thích
    Nếu đây là lần đầu tiên bạn làm việc với Arduino, chúng tôi chắc chắn khuyên bạn nên xem [Bắt đầu với Arduino](http://wiki.seeedstudio.com/Getting_Started_with_Arduino/) trước khi bắt đầu.

#### Vật liệu thiết yếu

| Seeeduino V4.2 | Base Shield| Grove-Button **x2** |Grove-Relay|
|--------------|-------------|-----------------|-----|
|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_1.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_4.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Relay/raw/master/img/button_s.jpg)|![](https://github.com/SeeedDocument/Grove-Relay/raw/master/img/Thumbnail.jpg)|
|<a href="http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html" target="_blank">Get One Now</a>|<a href="https://www.seeedstudio.com/Base-Shield-V2-p-1378.html" target="_blank">Get One Now</a>|<a href="https://www.seeedstudio.com/Grove-Button-p-766.html" target="_blank">Get One Now</a>|<a href="https://www.seeedstudio.com/Grove-Relay-p-769.html" target="_blank">Get One Now</a>|



!!!chú ý
    **1** Vui lòng cắm cáp USB nhẹ nhàng, nếu không bạn có thể làm hỏng cổng. Vui lòng sử dụng cáp USB có 4 dây bên trong, cáp 2 dây không thể truyền dữ liệu. Nếu bạn không chắc chắn về dây bạn có, bạn có thể nhấp vào [đây](https://www.seeedstudio.com/Micro-USB-Cable-48cm-p-1475.html) để mua.
    
    **2** Each Grove module comes with a Grove cable when you buy. In case you lose the Grove cable, you can click [here](https://www.seeedstudio.com/Grove-Universal-4-Pin-Buckled-20cm-Cable-%285-PCs-pack%29-p-936.html) to buy



#### Phần cứng

- **Bước 1.** Kết nối Grove-Relay tới **D4** của Grove-Base Shield.

- **Bước 2.** Kết nối Grove-Button#1 tới **D2** của Grove-Base Shield, Kết nối Grove-Button#2 tới cổng **D3** của Grove-Base Shield. 

- **Bước 3.** Cắm Grove - Base Shield vào Seeeduino.

- **Bước 4.** Kết nối Seeeduino tới PC qua một cáp USB.

![enter image description here](https://github.com/SeeedDocument/Grove-Relay/raw/master/img/button-relay.jpg)


!!!Chú ý
Nếu chúng tôi không có Grove Base Shield, chúng tôi cũng có thể kết nối trực tiếp Grove-Relay và Grove-Button tới mạch Arduino. Vui lòng nối như bên dưới.

| Grove-Relay | Arduino | Grove Cable|
|-------------|---------|-----------|
| GND         | GND     | Đen|
| VCC         | 5V      |Đỏ|
| SIG         | D4      |Vàng|

| Grove-Button#1 | Arduino |Grove Cable|
|----------------|---------|-------|
| GND            | GND     |Đen|
| VCC            | 5V      |Đỏ|
| SIG            | D2      |Vàng|

| Grove-Button#2 | Arduino |Grove Cable|
|----------------|---------|----|
| GND            | GND     |Đen|
| VCC            | 5V      |Đỏ|
| SIG            | D3      |Vàng|




#### Phần mềm


Dưới đây là bản demo cho bạn thấy cách điều khiển Grove - Relay bằng Grove - Nút. Khi nhấn một nút, rơle sẽ đóng lại. Khi nhấn nút khác, rơle sẽ mở.

- **Bước 1.** Mở Arduino IDE và sao chép mã sau vào một sketch mới.


```
// Relay Control

void setup()
{
  pinMode(2, INPUT);
  pinMode(3, INPUT);
  pinMode(4, OUTPUT);
}

void loop()
{
  if (digitalRead(2)==HIGH)
  {
    digitalWrite(4, HIGH);
    delay(100);
  }
  if (digitalRead(3)==HIGH)
  {
    digitalWrite(4, LOW);
  }
}

```

- **Bước 2.** Tải lên bản demo. Nếu bạn không biết cách tải lên mã, vui lòng kiểm tra [Cách tải lên mã](http://wiki.seeedstudio.com/Upload_Code/).


Tải lên xong, nếu bạn nhấn nút số 1 thì rơle sẽ được bật; và nếu bạn nhấn nút số 2 thì rơle sẽ tắt.


### Với Codecraft

#### Phần cứng

**Bước 1.** Kết nối Grove - Relay tới D4, kết nối hai Grove - Button tới D2 và D3 của Base Shield.

**Bước 2.** Cắm Base Shield tới Seeeduino/Arduino.

**Bước 3.** Kết nối Seeeduino/Arduino tới PC qua cáp USB.

#### Phần mềm

**Bước 1.** Mở [Codecraft](https://ide.chmakered.com/), thêm hỗ trợ Arduino và kéo một lệnh chính vào vùng làm việc.

!!!Chú ý
   Nếu đây là lần đầu tiên bạn sử dụng Codecraft, hãy xem thêm [Hướng dẫn sử dụng Codecraft bằng Arduino](http://wiki.seeedstudio.com/Guide_for_Codecraft_using_Arduino/)

**Bước 2.** Kéo các khối như hình dưới đây hoặc mở tệp cdc có thể được tải xuống ở cuối trang này.

![cc](https://raw.githubusercontent.com/SeeedDocument/Grove-Relay/master/img/cc_Relay.png)

Tải chương trình lên Arduino / Seeeduino của bạn.

!!!Kết quả
    Khi mã được tải lên. Rơle sẽ bật khi bạn nhấn nút được kết nối với cổng D2 và nó sẽ tắt khi bạn nhấn nút được kết nối với cổng D3.


### Đối với Raspberry Pi (Với Grove Base Hat cho Raspberry Pi)

#### Phần cứng

- **Bước 1**. Các thứ được sử dụng trong dự án:

| Raspberry pi | Grove Base Hat for RasPi| Grove - Relay |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Base_Hat_for_Raspberry_Pi/raw/master/img/thumbnail.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Relay/raw/master/img/Thumbnail.jpg)|
|[Get ONE Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Base-Hat-for-Raspberry-Pi-p-3186.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Relay-p-769.html)|

- **Bước 2**. Cắm Grove Base Hat vào Raspberry.
- **Bước 3**. Kết nối Grove - Relay tới cổng 12 của Base Hat.
- **Bước 4**. Kết nối Raspberry Pi tới PC qua cáp USB.


![](https://github.com/SeeedDocument/Grove-Relay/raw/master/img/Relay_Hat.jpg)

!!! Chú ý
    Đối với bước 3, bạn có thể kết nối cảm biến nhiệt độ và độ ẩm với **bất kỳ Cổng GPIO nào** nhưng đảm bảo bạn thay đổi lệnh với số cổng tương ứng.


#### Phần mềm

- **Step 1**. Theo dõi [Cài đặt phần mềm](http://wiki.seeedstudio.com/Grove_Base_Hat_for_Raspberry_Pi/#installation) để cấu hình môi trường phát triển.
- **Step 2**. Tải xuống tệp nguồn bằng cách nhân bản thư viện grove.py. 

```
cd ~
git clone https://github.com/Seeed-Studio/grove.py

```

- **Bước 3**. Thực hiện các lệnh dưới đây để chạy mã.

```
cd grove.py/grove
python grove_relay.py 12

```

Dưới đây là mã grove_relay.py.

```python

from grove.gpio import GPIO


class GroveRelay(GPIO):
    def __init__(self, pin):
        super(GroveRelay, self).__init__(pin, GPIO.OUT)

    def on(self):
        self.write(1)

    def off(self):
        self.write(0)


Grove = GroveRelay


def main():
    import sys
    import time

    if len(sys.argv) < 2:
        print('Usage: {} pin'.format(sys.argv[0]))
        sys.exit(1)

    relay = GroveRelay(int(sys.argv[1]))

    while True:
        try:
            relay.on()
            time.sleep(1)
            relay.off()
            time.sleep(1)
        except KeyboardInterrupt:
            relay.off()
            print("exit")
            exit(1)            

if __name__ == '__main__':
    main()



```

!!!Kết quả
    Nếu mọi thứ suôn sẻ, bạn sẽ thấy LED nhấp nhát.

Bạn có thể thoát chương trình này đơn giản bằng cách nhấn ++ ctrl + c ++.

### Đối với Raspberry Pi (với GrovePi_Plus)

#### Phần cứng

**Vật liệu thiết yếu**

| Raspberry pi | GrovePi_Plus| Grove-Button  |Grove-Relay|
|--------------|-------------|-----------------|-----|
|![enter image description here](https://github.com/SeeedDocument/Grove_Ultrasonic_Ranger/raw/master/img/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Ultrasonic_Ranger/raw/master/img/Grovepi%2B.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Relay/raw/master/img/button_s.jpg)|![](https://github.com/SeeedDocument/Grove-Relay/raw/master/img/Thumbnail.jpg)|
|<a href="https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html" target="_blank">Get One Now</a>|<a href="https://www.seeedstudio.com/GrovePi%2B-p-2241.html" target="_blank">Get One Now</a>|<a href="https://www.seeedstudio.com/Grove-Button-p-766.html" target="_blank">Get One Now</a>|<a href="https://www.seeedstudio.com/Grove-Relay-p-769.html" target="_blank">Get One Now</a>|



- **Bước 1.** Cắm GrovePi_Plus vào Raspberry.

- **Bước 2.** Kết nối Grove-Relay tới cổng **D4** của GrovePi_Plus.

- **Bước 3.** Kết nối Grove-Button tới cổng **D3** của GrovePi_Plus.

- **Bước 4.** Kết nối Raspberry tới PC qua cáp USB.


![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove-Relay/master/img/GrovePiPlus_Grove_relay.jpeg)

#### Phần mềm

Nếu đây là lần đầu tiên bạn sử dụng GrovePi, vui lòng thực hiện từng bước này. Nếu bạn là một người bạn cũ với GrovePi, bạn có thể bỏ qua ** Bước 1 ** và ** Bước2 **.


- **Bước 1.** Thiết lập phần mềm. Trong dòng lệnh, gõ các lệnh sau:

```
sudo curl -kL dexterindustries.com/update_grovepi | bash

```

```
sudo reboot
```

```
cd /home/pi/Desktop
```
```
git clone https://github.com/DexterInd/GrovePi.git
```

Để biết thêm chi tiết về phần này, vui lòng tham khảo [Cài đặt phần mềm](https://www.dexterindustries.com/GrovePi/get-started-with-the-grovepi/setting-software/).


- **Bước 2.** Thực hiện theo [Cập nhật Firmware](https://www.dexterindustries.com/GrovePi/get-started-with-the-grovepi/updating-firmware/) để cập nhật firmware mới nhất của GrovePi.


!!!Chú ý
    Chúng tôi đề nghị bạn cập nhật chương trình firmware hoặc đối với một số cảm biến bạn có thể gặp lỗi.


- **Bước 3.** Chạy lệnh sau để có kết quả.

```
cd /home/pi/Desktop/GrovePi/Software/Python/
sudo python grove_switch_relay.py
```


Nếu bạn muốn kiểm tra mã, bạn có thể sử dụng lệnh sau:

```
sudo nano grove_switch_relay.py

```

Code :

```python
# Raspberry Pi + Grove Switch + Grove Relay

import time
import grovepi
# Connect the Grove Switch to digital port D3
# SIG,NC,VCC,GND

switch = 3
# Connect the Grove Relay to digital port D4
# SIG,NC,VCC,GND

relay = 4
grovepi.pinMode(switch,"INPUT")
grovepi.pinMode(relay,"OUTPUT")
while True:
    try:
        if grovepi.digitalRead(switch):
            grovepi.digitalWrite(relay,1)
        else:
            grovepi.digitalWrite(relay,0)
            time.sleep(.05)
    except KeyboardInterrupt:
        grovepi.digitalWrite(relay,0)
        break
    except IOError:
        print "Error"
```



### Với TI LaunchPad

Điều khiển các thiết bị điện tử khác (Rơle)

![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove-Relay/master/img/Relay.jpg)

Ví dụ này cho thấy cách sử dụng mô-đun Grove-rơ-le để kiểm soát tải lớn hơn, tức là đèn bàn. Tín hiệu điện áp 3V có thể khiến rơle bật, cho phép dòng điện chạy qua thiết bị được kết nối.

```
/*
Relay
The basic Energia example.
This example code is in the public domain.
*/

#define RELAY_PIN 39

// the setup routine runs once when you press reset:
void setup() {
         pinMode(RELAY_PIN, OUTPUT); // initialize the digital pin as an output.
}

// the loop routine runs over and over again forever:
void loop() {
         digitalWrite(RELAY_PIN, HIGH); // turn the relay on (HIGH is the voltage level)
         delay(1000);   // wait for a second
         digitalWrite(RELAY_PIN, LOW);   // turn the relay o by making the voltage LOW
         delay(1000);   // wait for a second
}
```


## Nguồn

* **[Eagle]** [Grove - Relay Schematic and PCB in Eagle format](https://raw.githubusercontent.com/SeeedDocument/Grove-Relay/master/res/Grove-Relay_Eagle_Files.zip)
* **[PDF]** [Grove - Relay PCB in PDF format](https://github.com/SeeedDocument/Grove-Relay/raw/master/res/Grove%20-%20Relay%20PCB.pdf)
* **[PDF]** [Grove - Relay Schematic in PDF format](https://github.com/SeeedDocument/Grove-Relay/raw/master/res/Grove%20-%20Relay%20Schematic.pdf)
* **[Datasheet]** [HLS8-T73 Series Relay Datasheet](https://raw.githubusercontent.com/SeeedDocument/Grove-Relay/master/res/Relay_Datasheet.pdf)
* **[Codecraft]** [CDC File](https://raw.githubusercontent.com/SeeedDocument/Grove-Relay/master/res/Grove_Relay_CDC_File.zip)

## Dự án

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:0px;overflow:hidden;word-break:normal;}
.tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:0px;overflow:hidden;word-break:normal;}
.tg .tg-yw4l{vertical-align:top}
</style>
<table class="tg">
  <tr>
    <th class="tg-031e"><iframe frameborder='0' height='327.5' scrolling='no' src='https://project.seeedstudio.com/sodaqmoja/using-a-switch-to-open-and-close-a-relay-3329ec/embed' width='350'></iframe></th>
    <th class="tg-031e"><iframe frameborder='0' height='327.5' scrolling='no' src='https://project.seeedstudio.com/rei-vilo/private-iot-with-blynk-on-local-server-619926/embed' width='350'></iframe></th>
    <th class="tg-yw4l"><iframe frameborder='0' height='327.5' scrolling='no' src='https://project.seeedstudio.com/josephroberts/resinified-office-lock-0ca2eb/embed' width='350'></iframe></th>
  </tr>
</table>

**Module Relay Grove**:
 
<iframe width="560" height="315" src="https://www.youtube.com/embed/DnHqh_Rupb8" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/JOsjUOI9FU8" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

## Hỗ trợ kỹ thuật
Vui lòng gửi bất kỳ vấn đề kỹ thuật vào [diễn đàn](http://forum.seeedstudio.com/) của chúng tôi. <br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>