---
name: Grove - PIR Motion Sensor
category: Sensor
bzurl: https://www.seeedstudio.com/Grove-PIR-Motion-Sensor-p-802.html
oldwikiname: Grove - PIR Motion Sensor
prodimagename: Breakout_for_LinkIt_Smart_7688_v2.0_product_view_700.jpg
surveyurl: https://www.surveymonkey.com/r/grove-pir-motion-sensor
sku: 101020020
tags: io_3v3, io_5v, plat_duino, plat_pi
---


![](https://github.com/SeeedDocument/Grove_PIR_Motion_Sensor/raw/master/img/Grove_-_PIR_Motion_Sensor.jpg)

Cảm biến này cho phép bạn cảm nhận chuyển động, thường là chuyển động của con người trong phạm vi của nó. Chỉ cần kết nối nó với Grove - Base Shield và lập trình cho nó, khi bất kỳ ai di chuyển trong phạm vi phát hiện của nó, cảm biến sẽ xuất ra CAO trên chân SIG của nó.

<p style=":center"><a href="https://www.seeedstudio.com/Grove-PIR-Motion-Sensor-p-802.html" target="_blank"><img src="https://raw.githubusercontent.com/SeeedDocument/Seeed-WiKi/master/docs/images/get_one_now_small.png" width="210" height="41"  border=0 /></a></p>

## Đặc tính

- Giao diện tương thích Grove
- Điều chỉnh khoảng cách phát hiện
- Điều chỉnh thời gian giữ

!!!Mẹo
    Thông tin chi tiết về các module Grove vui lòng tham khảo [Hệ thống Grove](http://wiki.seeedstudio.com/Grove_System/)

## Các thông số kỹ thuật

|Tham số|Giá trị
|---|---|
|Điện áp hoạt động|	3V–5V
|Dòng hoạt động(VCC = 3V)|	100uA
|Dòng hoạt động(VCC = 5V)|	150uA
|Dải đo	|0.1 - 6m
|Khoảng cách phát hiện mặc định|	3m
|Thời gian giữ	|1 - 25s
|Chiều dài sóng làm việc	|7 - 14um
|Góc phát hiện|	120 degrees

## Các nền tảng được hỗ trợ


| Arduino                                                                                             | Raspberry Pi                                                                                             | BeagleBone                                                                                      | Wio                                                                                               | LinkIt ONE                                                                                         |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/arduino_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/raspberry_pi_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/bbg_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/wio_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/linkit_logo_n.jpg) |

!!!Chú ý
    Các nền tảng được đề cập ở trên được hỗ trợ như chỉ dẫn của phần mềm của module hoặc khả năng tương thích về mặt lý thuyết. Chúng tôi chỉ cung cấp thư viện phần mềm hoặc các ví dụ cho nền tảng Arduino trong hầu hết các trường hợp. Không thể cung cấp thư viện phần mềm / mã demo cho tất cả các nền tảng MCU. Do đó, người dùng phải viết thư viện phần mềm của riêng họ.
## Getting Started

!!!Chú thích
    Nếu đây là lần đầu tiên bạn làm việc với Arduino, chúng tôi chắc chắn khuyên bạn nên xem [Bắt đầu với Arduino](http://wiki.seeedstudio.com/Getting_Started_with_Arduino/) trước khi bắt đầu.

### Đối với Arduino

#### Phần cứng


- **Bước 1.** Chuẩn bị những thứ dưới đây:

| Seeeduino V4.2 | Grove - PIR Motion Sensor | Base Shield |
|--------------|----------------------|-----------------|
|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_1.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_PIR_Motion_Sensor/raw/master/img/Grove%20-%20PIR%20Motion%20Sensor_s.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_4.jpg)|
|[Get One Now](http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html)|[Get One Now](https://www.seeedstudio.com/Grove-PIR-Motion-Sensor-p-802.html)|[Get One Now](https://www.seeedstudio.com/Base-Shield-V2-p-1378.html)|


- **Bước 2.** Kết nối Grove - PIR Motion Sensor tới cổng **D2** của Grove-Base Shield.

- **Bước 3.** Cắm Grove - Base Shield vào Seeeduino.

- **Bước 4.** Kết nối Seeeduino tới PC qua một cáp USB.


![](https://github.com/SeeedDocument/Grove_PIR_Motion_Sensor/raw/master/img/connect_arduino.jpg)

!!!Chú ý
Nếu chúng tôi không có Grove Base Shield, chúng tôi cũng có thể kết nối trực tiếp Grove-PIR Motion Sensor tới Seeeduino như dưới đây.

| Seeeduino       | Grove - PIR Motion Sensor |
|---------------|-------------------------|
| 5V           | Đỏ                     |
| GND           | Đen                   |
| Không kết nối | Trắng                   |
| D2            | Vàng                  |



#### Phần mềm

- Sao chép mã dưới đây vào Arduino IDE và tải lên. Nếu bạn không biết cách tải lên mã, vui lòng kiểm tra [cách tải lên mã](http://wiki.seeedstudio.com/Upload_Code/).


```c
/*macro definitions of PIR motion sensor pin and LED pin*/
#define PIR_MOTION_SENSOR 2//Use pin 2 to receive the signal from the module


void setup()
{
    pinMode(PIR_MOTION_SENSOR, INPUT);
    Serial.begin(9600);  

}

void loop()
{
    if(digitalRead(PIR_MOTION_SENSOR))//if it detects the moving people?
        Serial.println("Hi,people is coming");
    else
        Serial.println("Watching");

 delay(200);
}

```


!!!Chú thích
     Khoảng cách phát hiện và thời gian giữ có thể được điều chỉnh bằng cách thêm hai chiết áp trên tàu. Để biết chi tiết xin vui lòng tham khảo Đại bàng V1.2 dưới đây. Module cũng có thể được đặt thành có thể điều chỉnh lại hoặc không thể điều chỉnh được bằng cách thay đổi mũ nhảy.

Kết quả:


![](https://github.com/SeeedDocument/Grove_PIR_Motion_Sensor/raw/master/img/result_arduino.png)

### Đối với Codecraft

#### Phần cứng

**Bước 1.** Kết nối Grove - PIR Motion Sensor tới cổng D2 của Base Shield.

**Bước 2.** Cắm Base Shield tới Seeeduino/Arduino.

**Bước 3.** Kết nối Seeeduino/Arduino tới PC qua cáp USB.

#### Phần mềm

**Bước 1.** Mở [Codecraft](https://ide.chmakered.com/), thêm hỗ trợ Arduino và kéo một lệnh chính vào vùng làm việc.

!!!Chú ý
   Nếu đây là lần đầu tiên bạn sử dụng Codecraft, hãy xem thêm [Hướng dẫn sử dụng Codecraft bằng Arduino](http://wiki.seeedstudio.com/Guide_for_Codecraft_using_Arduino/).

**Bước 2.** Kéo các khối như hình dưới đây hoặc mở tệp cdc có thể được tải xuống ở cuối trang này.

![cc](https://raw.githubusercontent.com/SeeedDocument/Grove_PIR_Motion_Sensor/master/img/cc_PIR_Motion_Sensor.png)

Tải chương trình lên Arduino / Seeeduino của bạn.

!!!Kết quả
   Khi mã được tải lên, LED tiếp tục sáng khi có người đang đến.

### Đối với Raspberry Pi (Với Grove Base Hat cho Raspberry Pi)

#### Phần cứng

- **Bước 1**. Các thứ được sử dụng trong dự án:

| Raspberry pi | Grove Base Hat for RasPi| Grove - PIR Motion Sensor |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Base_Hat_for_Raspberry_Pi/raw/master/img/thumbnail.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_PIR_Motion_Sensor/raw/master/img/Grove%20-%20PIR%20Motion%20Sensor_s.jpg)|
|[Get ONE Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Base-Hat-for-Raspberry-Pi-p-3186.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-PIR-Motion-Sensor-p-802.html)|

- **Bước 2**. Cắm Grove Base Hat vào Raspberry.
- **Bước 3**. Kết nối PIR motion sensor tới cổng 12 của Base Hat.
- **Bước 4**. Kết nối Raspberry Pi tới PC qua cáp USB.

![](https://github.com/SeeedDocument/Grove_PIR_Motion_Sensor/raw/master/img/Motion_Hat.jpg)

!!! Chú ý
    Đối với bước 3, bạn có thể kết nối cảm biến nhiệt độ và độ ẩm với **bất kỳ Cổng GPIO nào** nhưng đảm bảo bạn thay đổi lệnh với số cổng tương ứng.


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
python grove_mini_pir_motion_sensor.py 12

```

Dưới đây là mã grove_mini_pir_motion_sensor.py.

```python

import time
from grove.gpio import GPIO


class GroveMiniPIRMotionSensor(GPIO):
    def __init__(self, pin):
        super(GroveMiniPIRMotionSensor, self).__init__(pin, GPIO.IN)
        self._on_detect = None

    @property
    def on_detect(self):
        return self._on_detect

    @on_detect.setter
    def on_detect(self, callback):
        if not callable(callback):
            return

        if self.on_event is None:
            self.on_event = self._handle_event

        self._on_detect = callback

    def _handle_event(self, pin, value):
        if value:
            if callable(self._on_detect):
                self._on_detect()

Grove = GroveMiniPIRMotionSensor


def main():
    import sys

    if len(sys.argv) < 2:
        print('Usage: {} pin'.format(sys.argv[0]))
        sys.exit(1)

    pir = GroveMiniPIRMotionSensor(int(sys.argv[1]))

    def callback():
        print('Motion detected.')

    pir.on_detect = callback

    while True:
        time.sleep(1)


if __name__ == '__main__':
    main()

```

!!!success
    If everything goes well, you will be able to see the following result

```python

pi@raspberrypi:~/grove.py/grove $ python grove_mini_pir_motion_sensor.py 12
Motion detected.
Motion detected.
Motion detected.
^CTraceback (most recent call last):
  File "grove_mini_pir_motion_sensor.py", line 84, in <module>
    main()
  File "grove_mini_pir_motion_sensor.py", line 80, in main
    time.sleep(1)
KeyboardInterrupt

```

Bạn có thể thoát chương trình này đơn giản bằng cách nhấn ++ ctrl + c ++.


### Đối với Raspberry Pi (với GrovePi_Plus)

#### Phần cứng

- **Bước 1.** Chuẩn bị những thứ dưới đây:

| Raspberry pi | GrovePi_Plus | Grove - PIR Motion Sensor |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/Grove_Ultrasonic_Ranger/raw/master/img/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Ultrasonic_Ranger/raw/master/img/Grovepi%2B.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_PIR_Motion_Sensor/raw/master/img/Grove%20-%20PIR%20Motion%20Sensor_s.jpg)|
|[Get One Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get One Now](https://www.seeedstudio.com/GrovePi%2B-p-2241.html)|[Get One Now](https://www.seeedstudio.com/Grove-PIR-Motion-Sensor-p-802.html)|


- **Bước 2.** Cắm GrovePi_Plus vào Raspberry.

- **Step 3.** Kết nối cảm biến tới cổng **D8** của GrovePi_Plus.

- **Bước 4.** Kết nối Raspberry tới PC qua cáp USB.


![](https://github.com/SeeedDocument/Grove_PIR_Motion_Sensor/raw/master/img/connect_pi.jpg)

#### Phần mềm
- **Bước 1.** Theo dõi [Cài đặt phần mềm](https://www.dexterindustries.com/GrovePi/get-started-with-the-grovepi/setting-software/) để cài đặt môi trường phát triển.

- **Bước 2.** Thực hiện theo [Cập nhật Firmware](https://www.dexterindustries.com/GrovePi/get-started-with-the-grovepi/updating-firmware/) để cập nhật firmware mới nhất của GrovePi.

!!!Mẹo
    Trong wiki này, chúng tôi sử dụng đường dẫn **~/ GrovePi/** thay vì **/home/pi/Desktop/GrovePi**, bạn cần đảm bảo Bước 2 và Bước 3 sử dụng cùng một đường dẫn.

!!!Chú ý
    Chúng tôi đề nghị bạn cập nhật chương trình firmware hoặc đối với một số cảm biến bạn có thể gặp lỗi.


- **Bước 3.** Git nhân bản kho lưu trữ Github.

```
cd ~
git clone https://github.com/DexterInd/GrovePi.git

```

-	**Bước 4.** Chạy các lệnh bên dưới để sử dụng Cảm biến chuyển động Pir để theo dõi chuyển động của mọi người.

```
cd ~/GrovePi/Software/Python
sudo python grove_pir_motion_sensor.py
```

Đây là code grove_pir_motion_sensor.py.

```python
import time
import grovepi

# Connect the Grove PIR Motion Sensor to digital port D8
# SIG,NC,VCC,GND
pir_sensor = 8

grovepi.pinMode(pir_sensor,"INPUT")

while True:
    try:
        # Sense motion, usually human, within the target range
        if grovepi.digitalRead(pir_sensor):
            print 'Motion Detected'
        else:
            print '-'

        # if your hold time is less than this, you might not see as many detections
        time.sleep(.2)

    except IOError:
        print "Error"
```

Kết quả:

```python
pi@raspberrypi:~/GrovePi/Software/Python $ sudo python grove_pir_motion_sensor.py

-
-
-
Motion Detected
Motion Detected
Motion Detected
Motion Detected
Motion Detected
Motion Detected
Motion Detected
Motion Detected
Motion Detected
Motion Detected
Motion Detected
-
-

```

## FAQs

**Q1: Làm thế nào để làm cho khoảng cách điều chỉnh?**

A1: R2: được sử dụng để điều chỉnh khoảng cách phát hiện (hệ số AMP, 2MΩ). R6: được sử dụng để điều chỉnh thời gian giữ (nhiệm vụ kích hoạt, 100KΩ).

Khoảng cách phát hiện có thể được điều chỉnh từ 6 mét đến chỉ vài cm. Nếu chiết áp được đặt ở một đầu, mô-đun sẽ quá nhạy cảm để được kích hoạt bởi bầu khí quyển ngay cả khi không có người di chuyển trước nó. Thời gian giữ cũng có thể được điều chỉnh bằng chiết áp Delay_time, giá trị khoảng từ 25 đến 1 giây.

Nếu R2 và R6 được hàn, vui lòng đảm bảo R13 và R14 trống.

!!!Chú thích
     Có nguy cơ mạch có thể bị phá hủy. Hãy suy nghĩ kỹ trước khi thực hiện sửa đổi này.

![](https://github.com/SeeedDocument/Grove_PIR_Motion_Sensor/raw/master/img/Resistor.png)


## Nguồn


- **[Eagle]** [Grove - PIR Motion Sensor Eagle File v1.2](https://github.com/SeeedDocument/Grove_PIR_Motion_Sensor/raw/master/res/Grove%20PIR%20Motion%20Sensor_v1_2.zip)
- **[PDF]** [Grove - PIR Motion Sensor v1.2 Schematics](https://github.com/SeeedDocument/Grove_PIR_Motion_Sensor/raw/master/resources/Grove_PIR_Sensor_v1.2.pdf)
- **[PDF]** [Grove - PIR Motion Sensor Eagle V1.2 PCB](https://github.com/SeeedDocument/Grove_PIR_Motion_Sensor/raw/master/res/Grove%20-%20PIR%20motion%20sensor%20v1.1b%20PCB.pdf)
- **[Library]** [Github repository for PIR Motion Sensor](https://github.com/Seeed-Studio/PIR_Motion_Sensor)
- **[Datasheet]** [BISS0001 Datasheet](https://github.com/SeeedDocument/Grove_PIR_Motion_Sensor/raw/master/resources/Twig_-_BISS0001.pdf)
- **[Datasheet]** [Fresnel lens 8120 Datasheet](https://github.com/SeeedDocument/Grove_PIR_Motion_Sensor/raw/master/resources/Fresnel_lens_8120.pdf)
- **[Codecraft]** [CDC File](https://raw.githubusercontent.com/SeeedDocument/Grove_PIR_Motion_Sensor/master/res/Grove_PIR_Motion_Sensor_CDC_File.zip)


## Dự án

**Báo trộm với PIR Motion Sensor**: Bài viết này giải thích Báo động chống trộm với cảm biến chuyển động Pir.

<iframe frameborder='0' height='327.5' scrolling='no' src='https://www.hackster.io/pooja_baraskar/burglar-alarm-with-pir-motion-sensor-964c42/embed' width='350'></iframe>

## Hỗ trợ kỹ thuật
Vui lòng gửi bất kỳ vấn đề kỹ thuật vào [diễn đàn](http://forum.seeedstudio.com/) của chúng tôi.
<br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>