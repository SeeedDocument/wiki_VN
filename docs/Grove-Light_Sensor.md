---
name: Grove - Light Sensor
category: Sensor
bzurl: https://www.seeedstudio.com/Grove-Light-Sensor-(P)-v1.1-p-2693.html
oldwikiname: Grove_-_Light_Sensor
prodimagename: cover.jpg
sku: 101020173
tags: io_3v3, io_5v, plat_duino, plat_wio, plat_pi, plat_bbg, plat_linkit
---


![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/cover.jpg)


Cảm biến Grove - Light tích hợp một điện trở quang (điện trở phụ thuộc ánh sáng) để phát hiện cường độ ánh sáng. Điện trở của quang điện trở giảm khi cường độ ánh sáng tăng. Một chip OpAmp kép LM58 trên bo mạch tạo ra điện áp tương ứng với cường độ ánh sáng (tức là dựa trên giá trị điện trở). Tín hiệu đầu ra là giá trị tương tự, ánh sáng càng sáng thì giá trị càng lớn.
Module này có thể được sử dụng để xây dựng một công tắc điều khiển ánh sáng, tức là tắt đèn vào ban ngày và bật đèn vào ban đêm.

!!!Cảnh báo
     Giá trị cảm biến ánh sáng chỉ phản ánh xu hướng gần đúng của cường độ ánh sáng, nó KHÔNG đại diện cho Lumen chính xác.

<p style=":center"><a href="https://www.seeedstudio.com/Grove-Light-Sensor-v1.2-p-2727.html" target="_blank"><img src="https://raw.githubusercontent.com/SeeedDocument/Seeed-WiKi/master/docs/images/get_one_now_small.png" width="210" height="41"  border=0 /></a></p>

## Phiên bản

| Phiên bản sản phẩm              | Thay đổi                                                            | Ngày phát hành |
|------------------------------|--------------------------------------------------------------------|---------------|
| Grove - Light Sensor 1.0     | Ban đâu                                                            | 28/4/2013   |
| Grove - Light Sensor(P)      | Di chuyển kết nối Grove về phía sau                                  | 15/5/2014   |
| Grove - Light Sensor(P) V1.1 | Thay thế photoresistor-5528 bằng LS06-S Vs.Grove - Cảm biến ánh sáng (P)  | 31/12/2015   |
| Grove - Light Sensor 1.2     | Thay thế photoresistor-5528 bằng LS06-S Vs.Grove - Cảm biến ánh sáng 1.0 | 20/1/2016   |


## Đặc tính

* Giá trị đầu ra tương tự
* Độ nhạy và độ tin cậy cao
* Footprint nhỏ


* Nhận biết phổ rộng hơn

!!!Mẹo
    Thông tin chi tiết về các module Grove vui lòng tham khảo [Hệ thống Grove](http://wiki.seeedstudio.com/Grove_System/)

### Các nền tảng được hỗ trợ

| Arduino                                                                                             | Raspberry Pi                                                                                             | BeagleBone                                                                                      | Wio                                                                                               | LinkIt ONE                                                                                         |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/arduino_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/raspberry_pi_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/bbg_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/wio_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/linkit_logo.jpg) |

!!!Chú ý
    Các nền tảng được đề cập ở trên được hỗ trợ như chỉ dẫn của phần mềm của module hoặc khả năng tương thích về mặt lý thuyết. Chúng tôi chỉ cung cấp thư viện phần mềm hoặc các ví dụ cho nền tảng Arduino trong hầu hết các trường hợp. Không thể cung cấp thư viện phần mềm / mã demo cho tất cả các nền tảng MCU. Do đó, người dùng phải viết thư viện phần mềm của riêng họ.


## Các thông số kỹ thuật

|Item|Giá trị|
|-----|--------|
|Điện áp hoạt động|3~5V|
|Dòng hoạt động|	0.5~3 mA|
|Thời gian đáp ứng|20-30 ms|
|Bước sóng đỉnh|540 nm|
|Cân nặng|4 g|


## Getting Started

### Đối với Arduino

#### Phần cứng

- Bước 1. Chuẩn bị những thứ dưới đây:

| Seeeduino V4 | Base Shield |Grove - Light Sensor | Grove - LED Bar |
|--------------|----------------------|-----------------|---------------------|
|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_1.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_4.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Light_Sensor/raw/master/img/light_sensor_s.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_3.jpg)|
|[Get One Now](http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html)|[Get One Now](http://www.seeedstudio.com/Base-Shield-V2-p-1378.html)|[Get One Now](https://www.seeedstudio.com/Grove-Light-Sensor-v1.2-p-2727.html)|[Get One Now](http://www.seeedstudio.com/Grove-LED-Bar-v2.0-p-2474.html)|

- Bước 2. Kết nối cảm biến Grove-Light tới cổng A0 của Grove-Base Shield.
- Bước 3. Kết nối Grove-Led Bar tới cổng D2 của Grove-Base Shield.
- Bước 4. Cắm Grove - Base Shield vào Seeeduino.
- Bước 5. Kết nối Seeeduino tới PC qua một cáp USB.

![](https://github.com/SeeedDocument/Grove_Light_Sensor/raw/master/img/seeeduino_light.jpg)

!!Chú ý
Nếu chúng tôi không có Grove Base Shield,chúng tôi cũng có thể kết nối trực tiếp Grove-Light Sensor tới Seeeduino như dưới.

| Seeeduino       | Grove-Light Sensor |
|---------------|-------------------------|
| 5V           | Đỏ                     |
| GND           | Đen                   |
| Không nối | Trắng                   |
| A0            | Vàng                  |


| Seeeduino       | Grove-Led Bar |
|---------------|-------------------------|
| 5V            | Đỏ                     |
| GND           | Đen                    |
| D3            | Trắng                   |
| D2            | Vàng                  |

#### Phần mềm

- Bước 1. Tải xuống  [ Grove-LED Bar Library](https://github.com/Seeed-Studio/Grove_LED_Bar/archive/master.zip) từ Github.
- Bước 2. Tham khảo [How to install library](http://wiki.seeedstudio.com/How_to_install_Arduino_Library) để cài đặt thư viện cho Arduino.
- Bước 3. Sao chép mã vào Seeeduino IDE và tải lên.

```c

#include <Grove_LED_Bar.h>

Grove_LED_Bar bar(3, 2, 0);  // Clock pin, Data pin, Orientation

void setup()
{
  // nothing to initialize
  bar.begin();
  bar.setGreenToRed(true);
}

void loop()
{

  int value = analogRead(A0);
  value = map(value, 0, 800, 0, 10);

  bar.setLevel(value);
  delay(100);
}
```

- Bước 2. Thanh Led sẽ thay đổi dựa trên ánh sáng..

### Đối với Codecraft

#### Phần cứng

**Bước 1.** Kết nối Grove - Light Sensor tới cổng A0 của Base Shield.

**Bước 2.** Cắm Base Shield vào Seeeduino/Arduino của bạn.

**Bước 3.** Kết nối Seeeduino/Arduino tới PC qua cáp USB.

#### Phần mềm

**Bước 1.** Mở [Codecraft](https://ide.chmakered.com/), thêm hỗ trợ Arduino và kéo một lệnh chính vào vùng làm việc.

!!!Chú ý
   Nếu đây là lần đầu tiên bạn sử dụng Codecraft, hãy xem thêm [Hướng dẫn sử dụng Codecraft bằng Arduino](http://wiki.seeedstudio.com/Guide_for_Codecraft_using_Arduino/).

**Bước 2.** Kéo các khối như hình dưới đây hoặc mở tệp cdc có thể được tải xuống ở cuối trang này.

![cc](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/img/cc_Light_Sensor.png)

Tải chương trình lên Arduino / Seeeduino của bạn.

!!!Kết quả
   Khi mã được tải lên, bạn sẽ thấy giá trị độ sáng được hiển thị trong Serial Monitor.

### Đối với Raspberry Pi (Với Grove Base Hat cho Raspberry Pi)

#### Phần cứng

- **Bước 1**. Các thứ được sử dụng trong dự án:

| Raspberry pi | Grove Base Hat for RasPi| Grove - Light Sensor|
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Base_Hat_for_Raspberry_Pi/raw/master/img/thumbnail.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Light_Sensor/raw/master/img/light_sensor_s.jpg)|
|[Get ONE Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Base-Hat-for-Raspberry-Pi-p-3186.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Light-Sensor-v1.2-p-2727.html)|



- **Bước 2**. Cắm Grove Base Hat vào Raspberry.
- **Bước 3**. Kết nối cảm biến ánh sáng tới cổng A0 của Base Hat.
- **Bước 4**. Kết nối Raspberry Pi tới PC qua cáp USB.

![](https://github.com/SeeedDocument/Grove_Light_Sensor/raw/master/img/Light_Hat.jpg)


!!! Chú ý
    Đối với bước 3, bạn có thể kết nối cảm biến nhiệt độ và độ ẩm với **bất kỳ Cổng tương tự nào** nhưng đảm bảo bạn thay đổi lệnh với số cổng tương ứng.

#### Phần mềm

- **Bước 1**. Theo dõi [Cài đặt phần mềm](http://wiki.seeedstudio.com/Grove_Base_Hat_for_Raspberry_Pi/#installation) để cấu hình môi trường phát triển.
- **Bước 2**. Tải xuống tệp nguồn bằng cách nhân bản thư viện grove.py. 

```
cd ~
git clone https://github.com/Seeed-Studio/grove.py

```

- **Bước 3**. Thực hiện các lệnh dưới đây để chạy mã.

```
cd grove.py/grove
python grove_light_sensor_v1_2.py 0

```

Dưới đây là mã grove_light_sensor_v1_2.py.

```python

import math
import sys
import time
from grove.adc import ADC


class GroveLightSensor:

    def __init__(self, channel):
        self.channel = channel
        self.adc = ADC()

    @property
    def light(self):
        value = self.adc.read(self.channel)
        return value

Grove = GroveLightSensor


def main():
    if len(sys.argv) < 2:
        print('Usage: {} adc_channel'.format(sys.argv[0]))
        sys.exit(1)

    sensor = GroveLightSensor(int(sys.argv[1]))

    print('Detecting light...')
    while True:
        print('Light value: {0}'.format(sensor.light))
        time.sleep(1)

if __name__ == '__main__':
    main()

```

!!!Kết quả
    Nếu mọi thứ suôn sẻ, bạn sẽ thấy kết quả sau tương ứng với ánh sáng xung quanh
    
```python

pi@raspberrypi:~/grove.py/grove $ python grove_light_sensor_v1_2.py 0
Detecting light...
Light value: 600
Light value: 448
Light value: 267
Light value: 311
Light value: 102
Light value: 82
Light value: 63
Light value: 54
Light value: 49
Light value: 45
Light value: 545
^CTraceback (most recent call last):
  File "grove_light_sensor_v1_2.py", line 67, in <module>
    main()
  File "grove_light_sensor_v1_2.py", line 64, in main
    time.sleep(1)
KeyboardInterrupt

```
Bạn có thể thoát chương trình này đơn giản bằng cách nhấn ++ ctrl + c ++.

!!!Để ý
         Bạn có thể nhận thấy rằng đối với cổng analog, số pin màn hình có dạng như **A0, A1**, tuy nhiên trong lệnh chúng tôi sử dụng tham số **0** và **1**, giống như cổng kỹ thuật số . Vì vậy, hãy chắc chắn rằng bạn cắm mô-đun vào đúng cổng, nếu không có thể có xung đột pin.



### Đối với Raspberry Pi (với GrovePi_Plus)

#### Phần cứng

- Bước 1. Chuẩn bị những thứ dưới đây:

| Raspberry pi | GrovePi_Plus | Grove - Light Sensor | Grove - Red LED |
|--------------|-------------|-----------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/Grovepi%2B.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Light_Sensor/raw/master/img/light_sensor_s.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Red_LED/raw/master/img/Red%20LED_s.jpg)|
|[Get One Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get One Now](https://www.seeedstudio.com/GrovePi%2B-p-2241.html)|[Get One Now](https://www.seeedstudio.com/Grove-Light-Sensor-v1.2-p-2727.html)|[Get One Now](https://www.seeedstudio.com/s/Grove-Red-LED-p-1142.html)|

- Bước 2. Cắm GrovePi_Plus vào Raspberry.
- Bước 3. Kết nối cảm biến Grove-light tới cổng A0 của GrovePi_Plus.
- Bước 4. Kết nối Grove-Red Led tới cổng D4 của GrovePi_Plus.
- Bước 5. Kết nối Raspberry tới PC qua cáp USB.

![](https://github.com/SeeedDocument/Grove_Light_Sensor/raw/master/img/rasp_light.jpg)

#### Phần mềm

- Bước 1. Theo dõi [Cài đặt phần mềm](https://www.dexterindustries.com/GrovePi/get-started-with-the-grovepi/setting-software/) để cài đặt môi trường phát triển.
- Bước 2. Git nhân bản kho lưu trữ Github.

```
cd ~
git clone https://github.com/DexterInd/GrovePi.git

```

- Bước 3. Thực hiện lệnh dưới.


```
cd ~/GrovePi/Software/Python
python grove_light_sensor.py
```

Đây là code grove_light_sensor.py.

```python
import time
import grovepi

# Connect the Grove Light Sensor to analog port A0
# SIG,NC,VCC,GND
light_sensor = 0

# Connect the LED to digital port D4
# SIG,NC,VCC,GND
led = 4

# Turn on LED once sensor exceeds threshold resistance
threshold = 10

grovepi.pinMode(light_sensor,"INPUT")
grovepi.pinMode(led,"OUTPUT")

while True:
    try:
        # Get sensor value
        sensor_value = grovepi.analogRead(light_sensor)

        # Calculate resistance of sensor in K
        resistance = (float)(1023 - sensor_value) * 10 / sensor_value

        if resistance > threshold:
            # Send HIGH to switch on LED
            grovepi.digitalWrite(led,1)
        else:
            # Send LOW to switch off LED
            grovepi.digitalWrite(led,0)

        print("sensor_value = %d resistance = %.2f" %(sensor_value,  resistance))
        time.sleep(.5)

    except IOError:
        print ("Error")
```

- Bước 4. Đèn led sẽ bật khi cảm biến ánh sáng được che.

```
pi@raspberrypi:~/GrovePi/Software/Python $ python grove_light_sensor.py
sensor_value = 754 resistance = 3.57
sensor_value = 754 resistance = 3.57
sensor_value = 752 resistance = 3.60
sensor_value = 752 resistance = 3.60
sensor_value = 752 resistance = 3.60
sensor_value = 313 resistance = 22.68
sensor_value = 155 resistance = 56.00
sensor_value = 753 resistance = 3.59
```


## Nguồn

- **[Codecraft]** [CDC File](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/res/Grove_Light_Sensor_CDC_File.zip)
- **[Eagle&PDF]** [Eagle File for Grove - Light Sensor V1.0](https://github.com/SeeedDocument/Grove_Light_Sensor/raw/master/resources/Grove%20-%20Light%20Sensor.zip)
- **[Eagle&PDF]**  [Eagle File for Grove - Light Sensor(P) V1.0](https://github.com/SeeedDocument/Grove_Light_Sensor/raw/master/resources/Grove%20-%20Light%20Sensor%28P%29.zip)
- **[Eagle&PDF]**  [Eagle File for Grove - Light Sensor(P) V1.1](https://github.com/SeeedDocument/Grove_Light_Sensor/raw/master/resources/Grove%20-%20Light%20Sensor%28P%29%20v1.1.zip)
- **[Datasheet]** [LS06-MΦ5 Reference Information](https://github.com/SeeedDocument/Grove_Light_Sensor/raw/master/res/LS06-M%CE%A65_datasheet.pdf)
- **[Datasheet]**  [LM358.PDF](https://github.com/SeeedDocument/Grove_Light_Sensor/raw/master/res/LM358.pdf)
- **[More Reading]** Secret Box

![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/secret_box.png)

Ở đây chúng tôi sẽ cho bạn thấy một dự án được thực hiện với Grove - Light Sensor - Secret Box. Đầu tiên bạn cần một hộp, một hộp giấy, hộp gỗ, hộp nào cũng được. Đặt một cái gì đó vào hộp, vì chúng tôi đặt tên nó là hộp bí mật, điều đó có nghĩa là chúng tôi không muốn ai mở nó, nếu không sẽ có báo động để thông báo cho bạn.

Ở đây chúng tôi sử dụng LinkIt ONE làm bộ điều khiển, là một bo mạch tương thích với Arduino và bao gồm chức năng phong phú. Và bạn cần những thứ dưới đây:

* [LinkIt ONE](http://www.seeedstudio.com/LinkIt-ONE-p-2017.html)
* Grove - Light Sensor
* Grove - Base Shield
* Một thẻ sim

Hãy kết nối Grove - Light Sensor với A0 hoặc Base Shield và mở Arduino IDE, sao chép mã bên dưới và tải ví dụ lên LinkIt ONE. Sau đó, ai đó mở hộp, đèn sẽ phát hiện và gửi SMS cho bạn.

```c
// demo of Grove Starter kit for LinkIt ONE
// Secret box

#include <LGSM.h>

char num[20] = "13425171053";           // your number write here
char text[100] = "Warning: Your box had been opened!!";    // what do you want to send


const int pinLight = A0;                // light sensor connect to A0

bool isLightInBox()
{
    return (analogRead(pinLight)<50);   // when get data less than 50, means light sensor was in box
}

void setup()
{
    Serial.begin(115200);

    while(!isLightInBox());             // until put in box
    delay(2000);
}


void loop()
{
    if(!isLightInBox())                 // box is open
    {
        Serial.println("box had been opened");

        while(!LSMS.ready())
        {
            delay(1000);
        }

        Serial.println("SIM ready for work!");
        LSMS.beginSMS(num);
        LSMS.print(text);

        if(LSMS.endSMS())
        {
            Serial.println("SMS is sent");
        }
        else
        {
            Serial.println("SMS send fail");
        }

        while(!isLightInBox());             // until put in box
        delay(2000);
    }

    delay(10);
}
```

Chúc bạn thành công!

## Dự án

**Grove - Giới thiệu về cảm biến ánh sáng**:

<iframe frameborder='0' height='327.5' scrolling='no' src='https://www.hackster.io/ingo-lohs/grove-introduction-in-a-light-sensor-a55efd/embed' width='350'></iframe>

**Các khối môi trường! Biết vùng đất bên dưới Bạn sử dụng Sigfox**: Một khối lập phương với tất cả các cảm biến cần thiết, phù hợp cho một loạt các ứng dụng như nông nghiệp, giám sát, v.v.

<iframe frameborder='0' height='327.5' scrolling='no' src='https://www.hackster.io/dhairya-parikh/the-environment-cube-know-the-land-beneath-you-using-sigfox-952f29/embed' width='350'></iframe>


**Module Grove cảm biến ánh sáng**:
 
<iframe width="560" height="315" src="https://www.youtube.com/embed/ZvFswNYY2mU" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/GOROc2f5Xkg" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

## Hỗ trợ kỹ thuật
Vui lòng gửi bất kỳ vấn đề kỹ thuật vào [diễn đàn](http://forum.seeedstudio.com/) của chúng tôi. <br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>