---
category: Sensor
bzurl: https://www.seeedstudio.com/Grove-Ultrasonic-Ranger-p-960.html
oldwikiname: Grove - Ultrasonic Ranger
prodimagename: 350px-Ultrasonic_Ranger.jpg
surveyurl: https://www.research.net/r/Grove-Ultrasonic-Ranger
sku: 101020010
tags: io_3v3, io_5v, plat_duino, plat_pi
---
![](https://github.com/SeeedDocument/Grove_Ultrasonic_Ranger/raw/master/img/Ultrasonic.jpg)

Grove - Ultrasonic là module đo khoảng cách không tiếp xúc, hoạt động ở tần số 40KHz. Khi cung cấp tín hiệu kích hoạt xung với hơn 10uS thông qua chân tín hiệu, Grove_Ultráonic_Ranger sẽ phát ra 8 chu kỳ ở tần số 40kHz và phát hiện tiếng vang. Độ rộng xung của tín hiệu dội tỷ lệ với khoảng cách đo được. Đây là công thức: Khoảng cách = tín hiệu dội lại thời gian cao * Tốc độ âm thanh (340M / S) / 2. Grove_Ultrasonic_Ranger của trig và tín hiệu dội lại chia sẻ 1 chân SIG.

!!!Cảnh báo
	Không cắm nóng Grove-Ultrasonic-Ranger, nếu không nó sẽ làm hỏng cảm biến. Diện tích đo phải không dưới 0,5 mét vuông và mịn.

<p style=":center"><a href="https://www.seeedstudio.com/Grove-Ultrasonic-Ranger-p-960.html" target="_blank"><img src="https://raw.githubusercontent.com/SeeedDocument/Seeed-WiKi/master/docs/images/get_one_now_small.png" width="210" height="41"  border=0 /></a></p>

## Phiên bản

| Phiên bản sản phẩm              | Thay đổi                                                                                                                                                                                    | Ngày phát hành |
|------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|
| Grove-Ultrasonic ranger V1.0 | Ban đầu                                                                                                                                                                                    | 03/2012      |
| Grove-Ultrasonic ranger V2.0 | Cải thiện độ ổn định nguồn với bo mạch chính điện áp thấp với các thay đổi dưới đây: 1. Thêm tụ điện C14 2. Thiết kế lại bố cục để gọn gàng hơn 3. Tương thích với hệ thống điện áp 3.3V | 07/2017     |

## Các thông số kỹ thuật

|Tham số|	Phạm vi/Giá trị|
|:------|:------------------|
|Điện áp hoạt động|	3.2~5.2V|
|Dòng điện hoạt động|	8mA|
|Tần số siêu âm|	40kHz|
|Khoảng cách đo|	2-350cm|
|Độ phân giải|	1cm|
|Đầu ra|PWM|
|Kích thước|50mm X 25mm X 16mm|
|Cân nặng|13g|
|Góc đo|15°|
|Nhiệt độ làm việc|-10~60°C|
|Tín hiệu kích hoạt|10uS TTL|
|Tín hiệu dội lại |TTL|


!!!Mẹo
    Thông tin chi tiết về các module Grove vui lòng tham khảo [Hệ thống Grove](http://wiki.seeedstudio.com/Grove_System/)

## Các nền tảng được hỗ trợ

| Arduino                                                                                             | Raspberry Pi                                                                                             | BeagleBone                                                                                      | Wio                                                                                               | LinkIt ONE                                                                                         |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/arduino_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/raspberry_pi_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/bbg_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/wio_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/linkit_logo_n.jpg) |

!!!Chú ý
    Các nền tảng được đề cập ở trên được hỗ trợ như chỉ dẫn của phần mềm của module hoặc khả năng tương thích về mặt lý thuyết. Chúng tôi chỉ cung cấp thư viện phần mềm hoặc các ví dụ cho nền tảng Arduino trong hầu hết các trường hợp. Không thể cung cấp thư viện phần mềm / mã demo cho tất cả các nền tảng MCU. Do đó, người dùng phải viết thư viện phần mềm của riêng họ.


## Getting Started 

!!!Chú thích
    Nếu đây là lần đầu tiên bạn làm việc với Arduino, chúng tôi chắc chắn khuyên bạn nên xem [Bắt đầu với Arduino](http://wiki.seeedstudio.com/Getting_Started_with_Arduino/) trước khi bắt đầu.

### Đối với Arduino

#### Phần cứng

- **Bước 1.** Chuẩn bị những thứ dưới đây:

| Seeeduino V4.2 | Base Shield|  Grove - Ultrasonic Ranger |
|--------------|-------------|-----------------|
|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_1.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_4.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Ultrasonic_Ranger/raw/master/img/Ultrasonic_small.jpg)|
|[Get One Now](http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html)|[Get One Now](https://www.seeedstudio.com/Base-Shield-V2-p-1378.html)|[Get One Now](https://www.seeedstudio.com/Grove-Ultrasonic-Ranger-p-960.html)|

- **Bước 2.** Kết nối Ultrasonic Ranger tới cổng D7 của Grove-Base Shield.

- **Bước 3.** Cắm Grove - Base Shield vào Seeeduino.

- **Bước 4.** Kết nối Seeeduino tới PC qua một cáp USB.

![](https://github.com/SeeedDocument/Grove_Ultrasonic_Ranger/raw/master/img/arduino%20connection.jpg)

!!!Chú ý
Nếu chúng tôi không có Grove Base Shield, chúng tôi cũng có thể kết nối trực tiếp Grove - Ultrasonic_Ranger tới Seeeduino như dưới đây.

| Seeeduino       | Grove-Ultrasonic Ranger |
|---------------|-------------------------|
| 5V           | Đỏ                     |
| GND           | Đen                   |
| Không kết nối | Trắng                   |
| D7            | Vàng                  |

#### Phần mềm

- **Bước 1.** Tải xuống  [ thư viện UltrasonicRanger](https://github.com/Seeed-Studio/Grove_Ultrasonic_Ranger/archive/master.zip)  từ Github.
- **Bước 2.** Tham khảo [Cách cài đặt thư viện](http://wiki.seeedstudio.com/How_to_install_Arduino_Library) để cài đặt thư viện cho Arduino
- **Bước 3.** Sao chép mã vào Arduino IDE và tải lên. Nếu bạn không biết cách tải lên mã, vui lòng kiểm tra [cách tải mã lên](http://wiki.seeedstudio.com/Upload_Code/).

```
#include "Ultrasonic.h"

Ultrasonic ultrasonic(7);
void setup()
{
	Serial.begin(9600);
}
void loop()
{
	long RangeInInches;
	long RangeInCentimeters;

	Serial.println("The distance to obstacles in front is: ");
	RangeInInches = ultrasonic.MeasureInInches();
	Serial.print(RangeInInches);//0~157 inches
	Serial.println(" inch");
	delay(250);

	RangeInCentimeters = ultrasonic.MeasureInCentimeters(); // two measurements should keep an interval
	Serial.print(RangeInCentimeters);//0~400cm
	Serial.println(" cm");
	delay(250);
}
```

- **Bước 4.** Chúng ta sẽ thấy màn hình hiển thị khoảng cách trên thiết bị đầu cuối như dưới đây.

```
The distance to obstacles in front is:
2 inches
6 cm
The distance to obstacles in front is:
2 inches
6 cm
The distance to obstacles in front is:
2 inches
6 cm
```

### Đối với Codecraft

#### Phần cứng

**Bước 1.** Kết nối Grove - Ultrasonic Ranger tới cổng D7 của Base Shield.

**Bước 2.** Cắm Base Shield vào Seeeduino/Arduino của bạn.


**Bước 3.** Kết nối Seeeduino/Arduino tới PC qua cáp USB.

#### Phần mềm

**Bước 1.** Mở [Codecraft](https://ide.chmakered.com/), thêm hỗ trợ Arduino và kéo một lệnh chính vào vùng làm việc.

!!!Chú ý
   Nếu đây là lần đầu tiên bạn sử dụng Codecraft, hãy xem thêm [Hướng dẫn sử dụng Codecraft bằng Arduino](http://wiki.seeedstudio.com/Guide_for_Codecraft_using_Arduino/).

**Bước 2.** Kéo các khối như hình dưới đây hoặc mở tệp cdc có thể được tải xuống ở cuối trang này.

![cc](https://raw.githubusercontent.com/SeeedDocument/Grove_Ultrasonic_Ranger/master/img/cc_Ultrasonic_Ranger.png)

Tải chương trình lên Arduino / Seeeduino của bạn.

!!!Kết quả
    Khi mã được tải lên, bạn sẽ thấy có nước hay không trong Màn hình Nối tiếp.

### Đối với Raspberry Pi (Với Grove Base Hat cho Raspberry Pi)

#### Phần cứng

- **Bước 1**. Các thứ được sử dụng trong dự án:

| Raspberry pi | Grove Base Hat for RasPi| Grove - Ultrasonic Ranger |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Base_Hat_for_Raspberry_Pi/raw/master/img/thumbnail.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Ultrasonic_Ranger/raw/master/img/Ultrasonic_small.jpg)|
|[Get ONE Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Base-Hat-for-Raspberry-Pi-p-3186.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Ultrasonic-Ranger-p-960.html)|



- **Bước 2**. Cắm Grove Base Hat vào Raspberry.
- **Bước 3**. Kết nối Grove - Ultrasonic Ranger tới cổng D5 của Base Hat.
- **Bước 4**. Kết nối Raspberry Pi tới PC qua cáp USB.

![](https://github.com/SeeedDocument/Grove_Base_Hat_for_Raspberry_Pi/raw/master/img/connect2.jpg)


!!! Chú ý
    Đối với bước 3, bạn có thể kết nối ultrasonic ranger với **bất kỳ Cổng GPIO nào** nhưng đảm bảo bạn thay đổi lệnh với số cổng tương ứng.


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
python grove_ultrasonic_ranger.py 5 6

```

Dưới đây là code grove_ultrasonic_ranger.py.

```python

import sys
import time
from grove.gpio import GPIO

usleep = lambda x: time.sleep(x / 1000000.0)

_TIMEOUT1 = 1000
_TIMEOUT2 = 10000

class GroveUltrasonicRanger(object):
    def __init__(self, pin):
        self.dio =GPIO(pin)

    def _get_distance(self):
        self.dio.dir(GPIO.OUT)
        self.dio.write(0)
        usleep(2)
        self.dio.write(1)
        usleep(10)
        self.dio.write(0)

        self.dio.dir(GPIO.IN)

        t0 = time.time()
        count = 0
        while count < _TIMEOUT1:
            if self.dio.read():
                break
            count += 1
        if count >= _TIMEOUT1:
            return None

        t1 = time.time()
        count = 0
        while count < _TIMEOUT2:
            if not self.dio.read():
                break
            count += 1
        if count >= _TIMEOUT2:
            return None

        t2 = time.time()

        dt = int((t1 - t0) * 1000000)
        if dt > 530:
            return None

        distance = ((t2 - t1) * 1000000 / 29 / 2)    # cm

        return distance

    def get_distance(self):
        while True:
            dist = self._get_distance()
            if dist:
                return dist


Grove = GroveUltrasonicRanger


def main():
    if len(sys.argv) < 2:
        print('Usage: {} pin_number'.format(sys.argv[0]))
        sys.exit(1)

    sonar = GroveUltrasonicRanger(int(sys.argv[1]))

    print('Detecting distance...')
    while True:
        print('{} cm'.format(sonar.get_distance()))
        time.sleep(1)

if __name__ == '__main__':
    main()



```

!!!Kết quả
    Nếu mọi thứ suôn sẻ, bạn sẽ thấy kết quả sau.
    
```python

pi@raspberrypi:~/grove.py/grove $ python grove_ultrasonic_ranger.py 5 6
Detecting distance...
121.757901948 cm
246.894770655 cm
2.60205104433 cm
0.205533257846 cm
0.657706425108 cm
247.433267791 cm
122.485489681 cm
^CTraceback (most recent call last):
  File "grove_ultrasonic_ranger.py", line 110, in <module>
    main()
  File "grove_ultrasonic_ranger.py", line 107, in main
    time.sleep(1)
KeyboardInterrupt


```


Bạn có thể thoát chương trình này đơn giản bằng cách nhấn ++ ctrl + c ++.




### Đối với Raspberry Pi (với GrovePi_Plus)

#### Phần cứng

- **Bước 1.** Chuẩn bị những thứ dưới đây:

| Raspberry pi | GrovePi_Plus | Grove - Ultrasonic Ranger |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/Grove_Ultrasonic_Ranger/raw/master/img/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Ultrasonic_Ranger/raw/master/img/Grovepi%2B.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Ultrasonic_Ranger/raw/master/img/Ultrasonic_small.jpg)|
|[Get One Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get One Now](https://www.seeedstudio.com/GrovePi%2B-p-2241.html)|[Get One Now](https://www.seeedstudio.com/Grove-Ultrasonic-Ranger-p-960.html)|


- **Bước 2.** Cắm GrovePi_Plus vào Raspberry.
- **Bước 3.** Kết nối Grove-Ultrasonic_Ranger tới cổng **D4** của GrovePi_Plus.
- **Bước 4.** Kết nối Raspberry tới PC qua cáp USB.

![](https://github.com/SeeedDocument/Grove_Ultrasonic_Ranger/raw/master/img/pi%20connection.jpg)

#### Phần mềm

- **Bước 1.** Theo dõi [Cài đặt phần mềm](https://www.dexterindustries.com/GrovePi/get-started-with-the-grovepi/setting-software/) để cài đặt môi trường phát triển.
- **Bước 2.** Git nhân bản kho lưu trữ Github.
```
cd ~
git clone https://github.com/DexterInd/GrovePi.git

```

-	**Bước 3.** Thực hiện các lệnh dưới đây để sử dụng phạm vi siêu âm để đo khoảng cách.


```
cd ~/GrovePi/Software/Python
python grove_ultrasonic.py
```

Đây là code grove_ultrasonic.py.

```python
# GrovePi + Grove Ultrasonic Ranger

from grovepi import *

# Connect the Grove Ultrasonic Ranger to digital port D4
# SIG,NC,VCC,GND

ultrasonic_ranger = 4

while True:
    try:
        # Read distance value from Ultrasonic
        print ultrasonicRead(ultrasonic_ranger)

    except TypeError:
        print "Error"
    except IOError:
        print "Error"
```

- **Bước 4.** Chúng ta sẽ thấy màn hình hiển thị khoảng cách trên thiết bị đầu cuối như dưới đây.

```
pi@raspberrypi:~/GrovePi/Software/Python $ python grove_ultrasonic.py
9
9
9
9
9
9
9
9
9
9
9

```

## FAQs


**Q1: Cảm biến Grove-Ultrasonic hoạt động như thế nào?**

- A1: Khi chúng tôi cung cấp tín hiệu kích hoạt xung với hơn 10uS thông qua pin đơn, Grove_Ult siêu_Ranger sẽ phát ra 8 chu kỳ ở tần số 40kHz và phát hiện tiếng vang. Độ rộng xung của tín hiệu dội tỷ lệ với khoảng cách đo được. Đây là công thức: Khoảng cách = tín hiệu dội lại thời gian cao * Tốc độ âm thanh (340M / S) / 2.




**Q2: Tại sao cảm biến Grove-Ultrasonic chỉ có 1 chân tín hiệu, so sánh với các chân cảm biến siêu âm Trig và Echo khác?**

- A2:Grove_Ultrasonic_Ranger của tín hiệu trig và echo chia sẻ 1  chân SIG qua MCU.  


**Q3: Tôi có thể tìm hỗ trợ kỹ thuật ở đâu nếu tôi gặp một số vấn đề khác?**

- A3: Vui lòng gửi email đến techsupport@seeed.cc

**Q4: Chúng ta có thể kết nối siêu âm mulitule với một arduino không?**

- A4: Có, đây là ví dụ, một cảm biến được kết nối với D2 và khác với D3.

```c++
#include "Ultrasonic.h"

Ultrasonic ultrasonic1(2);
Ultrasonic ultrasonic2(3);
void setup()
{
    Serial.begin(9600);
}
void loop()
{
    long RangeInCentimeters1;
    long RangeInCentimeters2;

    RangeInCentimeters1 = ultrasonic1.MeasureInCentimeters(); // two measurements should keep an interval
    Serial.print(RangeInCentimeters1);//0~400cm
    Serial.println(" cm");
    
    RangeInCentimeters2 = ultrasonic2.MeasureInCentimeters(); // two measurements should keep an interval
    Serial.print(RangeInCentimeters2);//0~400cm
    Serial.println(" cm");
    
    delay(250);
}

```
 


## Nguồn

- **[PDF]** [Download Wiki PDF](https://github.com/SeeedDocument/Grove_Ultrasonic_Ranger/raw/master/res/Grove-Ultrasonic_Ranger_WiKi.pdf)
- **[PDF]** [Grove_Ultrasonic Ranger Schematic](https://github.com/SeeedDocument/Grove_Ultrasonic_Ranger/raw/master/res/Grove_Ultrasonic%20Ranger%20Schematic.pdf)
- **[PDF]** [Ceramic Ultrasonic Sensor NU40C16T/R-1](https://github.com/SeeedDocument/Grove_Ultrasonic_Ranger/blob/master/res/NU40C16T-R-1.pdf)
- **[Library]** [Grove_Ultrasonic Ranger library](https://github.com/Seeed-Studio/Grove_Ultrasonic_Ranger/archive/master.zip)
- **[Codecraft]** [CDC File](https://raw.githubusercontent.com/SeeedDocument/Grove_Ultrasonic_Ranger/master/res/Grove_Ultrasonic_Ranger_CDC_File.zip)
- **[Project]** [The Color Helix](https://community.seeedstudio.com/project_detail.html?id=138)
- **[Project]** [Indoor Lightning Cloud](https://community.seeedstudio.com/project_detail.html?id=182)
- **[Project]** [Automatic Water Level Controller](https://community.seeedstudio.com/project_detail.html?id=241)
- **[Example]** [Example_Measure_distance_and_led_display](https://github.com/SeeedDocument/Grove_Ultrasonic_Ranger/raw/master/res/Example_Measure_distance_and_led_display.zip)
- **[Example]** [Example_Measure_and_display_the_distance](https://github.com/SeeedDocument/Grove_Ultrasonic_Ranger/raw/master/res/Example_Measure_and_display_the_distance.zip)

## Dự án 

**Hack cầu thang tại văn phòng mới của Saeed**: Biến cầu thang tại văn phòng thành một cài đặt tương tác, và thậm chí là một cách tuyệt vời để truyền tải thông điệp "CHỈ NHÂN VIÊN" cho khách truy cập.

<iframe frameborder='0' height='327.5' scrolling='no' src='https://www.hackster.io/stairs-hackers/hacking-the-stairs-at-seeed-s-new-office-9ef30b/embed' width='350'></iframe>

## Hỗ trợ kỹ thuật
Vui lòng gửi bất kỳ vấn đề kỹ thuật vào [diễn đàn](http://forum.seeedstudio.com/) của chúng tôi.
<br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>