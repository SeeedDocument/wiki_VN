---
name: Grove - RTC
category: Sensor
bzurl: https://seeedstudio.com/Grove-RTC-p-758.html
oldwikiname: Grove_-_RTC
prodimagename: Grove-RTC.jpg
bzprodimageurl: http://statics3.seeedstudio.com/images/101020013 1.jpg
surveyurl: https://www.research.net/r/Grove-RTC
sku: 101020013
tags: grove_i2c, io_3v3, io_5v, plat_duino, plat_pi
---

![](https://github.com/SeeedDocument/Grove-RTC/raw/master/img/45d.jpg)

Module RTC dựa trên chip đồng hồ DS1307, hỗ trợ giao thức I2C. Nó sử dụng pin lithium (CR1225). Đồng hồ / lịch cung cấp giây, phút, giờ, ngày, ngày, tháng và năm. Ngày kết thúc của tháng được tự động điều chỉnh cho các tháng có ít hơn 31 ngày, bao gồm cả việc điều chỉnh cho các năm nhuận. Đồng hồ hoạt động ở định dạng 24 giờ hoặc 12 giờ với chỉ báo AM / PM. Và nó có giá trị đến 2100. Để có được hiệu suất mạnh mẽ, bạn phải đặt pin lithium 3-volt CR1225 vào ngăn chứa pin. Nếu bạn chỉ sử dụng nguồn điện chính, module có thể không hoạt động bình thường, vì tinh thể có thể không dao động.

[![](https://raw.githubusercontent.com/SeeedDocument/common/master/Get_One_Now_Banner.png)](https://www.seeedstudio.com/Grove-RTC-p-758.html)

<div class="admonition note">
<p class="admonition-title">Chú ý</p>
Pin không được bao gồm.
</div>

## Thông số kỹ thuật

-   Kích thước PCB: 2.0cm\*4.0cm
-   Giao diện: 2.0mm pitch pin header
-   Cấu trúc IO: SCL,SDA,VCC,GND
-   ROHS: YES
-   VCC：3.3~5.5V
-   Đầu vào mức cao logic ：2.2~VCC+0.3 V
-   Đầu vào mức thấp logic ：-0.3~+0.8 V
-   Điện áp pin：2.0~3.5 V

!!!Mẹo
    Thông tin chi tiết về các module Grove vui lòng tham khảo [Hệ thống Grove](http://wiki.seeedstudio.com/Grove_System/)

## Các nền tảng được hỗ trợ

| Arduino                                                                                             | Raspberry Pi                                                                                             | BeagleBone                                                                                      | Wio                                                                                               | LinkIt ONE                                                                                         |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/arduino_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/raspberry_pi_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/bbg_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/wio_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/linkit_logo_n.jpg) |

!!!Chú ý
    Các nền tảng được đề cập ở trên được hỗ trợ như chỉ dẫn của phần mềm của module hoặc khả năng tương thích về mặt lý thuyết. Chúng tôi chỉ cung cấp thư viện phần mềm hoặc các ví dụ cho nền tảng Arduino trong hầu hết các trường hợp. Không thể cung cấp thư viện phần mềm / mã demo cho tất cả các nền tảng MCU. Do đó, người dùng phải viết thư viện phần mềm của riêng họ.


## Getting Started


### Với Arduino

#### Phần cứng

- **Bước 1.** Chuẩn bị những thứ dưới đây:

| Seeeduino V4.2 | Base Shield| Grove-RTC |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/seeeduino_v4.2.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/base_shield.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-RTC/raw/master/img/45d_small.jpg)|
|[Get One Now](http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html)|[Get One Now](https://www.seeedstudio.com/Base-Shield-V2-p-1378.html)|[Get One Now](https://www.seeedstudio.com/Grove-RTC-p-758.html)|

- **Bước 2.** Kết nối Grove-RTC tới **I2C** của Grove-Base Shield.
- **Step 3.** Cắm Grove - Base Shield vào Seeeduino.
- **Step 4.** Kết nối Seeeduino tới PC qua một cáp USB.

<div class="admonition note">
<p class="admonition-title">Chú ý</p>
 Để đạt được hiệu suất cao, bạn phải đặt pin lithium 3-volt CR1225 vào ngăn chứa pin. Nếu bạn chỉ sử dụng nguồn điện chính, module có thể không hoạt động bình thường, vì tinh thể có thể không dao động.
</div>

![](https://github.com/SeeedDocument/Grove-RTC/raw/master/img/arduino_connection.jpg)

!!!Chú ý
Nếu chúng tôi không có Grove Base Shield, chúng tôi cũng có thể kết nối trực tiếp Grove-RTC tới mạch Arduino. Vui lòng kết nối như dưới đây.

| Seeeduino_v4 | Grove-RTC  |
|-------------|--------------------------|
| 5V          | VCC                      |
| GND         | GND                      |
| SDA         | SDA                      |
| SCL         | SCL                      |



#### Phần mềm
**Bước 1.** Tải xuống  [ Thư viện RTC](https://github.com/Seeed-Studio/RTC_DS1307/archive/master.zip).

**Step 2.**Tham khảo [How to install library](http://wiki.seeedstudio.com/How_to_install_Arduino_Library) để cài đặt thư viện cho Arduino.

**Bước 3.** Tạo một sketch Arduino mới và dán các mã bên dưới vào nó hoặc mở mã trực tiếp theo đường dẫn: **File -> Example ->RTC->SetTimeAndDisplay**.

  ![](https://github.com/SeeedDocument/Grove-RTC/raw/master/img/library%20example.jpg)


```c++     
#include <Wire.h>
#include "DS1307.h"

DS1307 clock;//define a object of DS1307 class
void setup()
{
    Serial.begin(9600);
    clock.begin();
    clock.fillByYMD(2013,1,19);//Jan 19,2013
    clock.fillByHMS(15,28,30);//15:28 30"
    clock.fillDayOfWeek(SAT);//Saturday
    clock.setTime();//write time to the RTC chip
}
void loop()
{
    printTime();
}
    /*Function: Display time on the serial monitor*/
void printTime()
{
    clock.getTime();
    Serial.print(clock.hour, DEC);
    Serial.print(":");
    Serial.print(clock.minute, DEC);
    Serial.print(":");
    Serial.print(clock.second, DEC);
    Serial.print("  ");
    Serial.print(clock.month, DEC);
    Serial.print("/");
    Serial.print(clock.dayOfMonth, DEC);
    Serial.print("/");
    Serial.print(clock.year+2000, DEC);
    Serial.print(" ");
    Serial.print(clock.dayOfMonth);
    Serial.print("*");
    switch (clock.dayOfWeek)// Friendly printout the weekday
    {
        case MON:
        Serial.print("MON");
        break;
        case TUE:
        Serial.print("TUE");
        break;
        case WED:
        Serial.print("WED");
        break;
        case THU:
        Serial.print("THU");
        break;
        case FRI:
        Serial.print("FRI");
        break;
        case SAT:
        Serial.print("SAT");
        break;
        case SUN:
        Serial.print("SUN");
        break;
    }
    Serial.println(" ");
}
```

**Step 4.**  Đặt thời gian. Thay đổi đối số chức năng thành ngày / giờ hiện tại. Vui lòng chú ý đến định dạng của đối số.

```c
clock.fillByYMD(2013,1,19);//Jan 19,2013
clock.fillByHMS(15,28,30);//15:28 30"
clock.fillDayOfWeek(SAT);//Saturday
```

**Step 5.** Tải lên mã và mở màn hình nối tiếp để nhận dữ liệu của cảm biến
![](https://github.com/SeeedDocument/Grove-RTC/raw/master/img/arduino%20result.png)



### Với Raspberry Pi

#### Phần cứng

- **Bước 1.** Chuẩn bị các thứ như dưới:


| Raspberry pi | GrovePi_Plus | Grove-RTC |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/Grovepi%2B.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-RTC/raw/master/img/45d_small.jpg)|
|[Get One Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get One Now](https://www.seeedstudio.com/GrovePi%2B-p-2241.html)|[Get One Now](https://www.seeedstudio.com/Grove-RTC-p-758.html)|



- **Step 2.** Cắm GrovePi_Plus vào Raspberry.
- **Step 3.** Kết nối Grove-RTC  tới **I2C** của GrovePi_Plus.
- **Step 4.** Kết nối Raspberry tới PC qua cáp USB.

![](https://github.com/SeeedDocument/Grove-RTC/raw/master/img/rasp_connection.jpg)

#### Phần mềm

- **Bước 1.** Theo dõi [Cài đặt phần mềm](http://wiki.seeedstudio.com/Grove_Base_Hat_for_Raspberry_Pi/#installation) để cấu hình môi trường phát triển.
- **Bước 2.** Git nhân bản kho lưu trữ Github.

```bash
cd ~
git clone https://github.com/DexterInd/GrovePi.git

```

-	**Bước 3.** Thực hiện các lệnh dưới đây để sử dụng cảm biến này.


```bash
cd ~/GrovePi/Software/Python
python grove_i2c_rtc.py
```
Đây là code

```Python
#!/usr/bin/env python
#
# GrovePi Example for using the Grove I2C RTC (http://www.seeedstudio.com/wiki/Grove_-_RTC)
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

# Connect the Grove Real Time Clock to any I2C port eg. I2C-1
# Can be found at I2C address 0x68
# SCL,SDA,VCC,GND

while True:
    try:
        print(grovepi.rtc_getTime())
        time.sleep(.5)

    except IOError:
        print ("Error")
```

-	**Bước 4.** Đây là kết quả.

  ![](https://github.com/SeeedDocument/Grove-RTC/raw/master/img/rpi_display.jpg)

**Demo 2: Grove_rtc**

Bạn cũng có thể sử dụng bản demo này để hiển thị thời gian chung. Vui lòng tạo grove_rtc.py và sao chép mã bên dưới.

```python
    '''
     * Grove-RTC.py
     * Demo for Raspberry Pi
     *
     * Copyright (c) 2014 seeed technology inc.
     * Website    : community.seeedstudio.com/
     * Author     : Lambor
     * Create Time: Nov 2014
     * Change Log :
     *
     * The MIT License (MIT)
     *
     * Permission is hereby granted, free of charge, to any person obtaining a copy
     * of this software and associated documentation files (the "Software"), to deal
     * in the Software without restriction, including without limitation the rights
     * to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
     * copies of the Software, and to permit persons to whom the Software is
     * furnished to do so, subject to the following conditions:
     *
     * The above copyright notice and this permission notice shall be included in
     * all copies or substantial portions of the Software.
     *
     * THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
     * IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
     * FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
     * AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
     * LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
     * OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
     * THE SOFTWARE.
     '''

    #!/usr/bin/python
import time
import smbus


    bus = smbus.SMBus(1)    # 0 = /dev/i2c-0 (port I2C0), 1 = /dev/i2c-1 (port I2C1)   

class DS1307():     
        def __init__(self):
            self.MON = 1
            self.TUE = 2
            self.WED = 3
            self.THU = 4
            self.FRI = 5
            self.SAT = 6
            self.SUN = 7
            self.DS1307_I2C_ADDRESS = 0x68

            print 'begin'

        def decToBcd(self, val):
            return ( (val/10*16) + (val%10) )

        def bcdToDec(self,  val):
            return ( (val/16*10) + (val%16) )

        def begin(self, news):
            print news

        def startClock(self):   
            bus.write_byte(self.DS1307_I2C_ADDRESS, 0x00)
            self.second = bus.read_byte(self.DS1307_I2C_ADDRESS) & 0x7f
            bus.write_byte_data(self.DS1307_I2C_ADDRESS, 0x00, self.second)

            print 'startClock..'

        def stopClock(self):                        
            bus.write_byte(self.DS1307_I2C_ADDRESS, 0x00)
            self.second = bus.read_byte(self.DS1307_I2C_ADDRESS) | 0x80
            bus.write_byte_data(self.DS1307_I2C_ADDRESS, 0x00, self.second)         

            print 'stopClock..'

        def setTime(self):
            data = [self.decToBcd(self.second), self.decToBcd(self.minute), \
                    self.decToBcd(self.hour), self.decToBcd(self.dayOfWeek), \
                    self.decToBcd(self.dayOfMonth), self.decToBcd(self.month), \
                    self.decToBcd(self.year)]

            bus.write_byte(self.DS1307_I2C_ADDRESS, 0x00)
            bus.write_i2c_block_data(self.DS1307_I2C_ADDRESS,0x00,data)

            print 'setTime..'

        def getTime(self):
            bus.write_byte(self.DS1307_I2C_ADDRESS, 0x00)
            data = bus.read_i2c_block_data(self.DS1307_I2C_ADDRESS,0x00)
            #A few of these need masks because certain bits are control bits
            self.second = self.bcdToDec(data[0] & 0x7f)
            self.minute = self.bcdToDec(data[1])
            self.hour = self.bcdToDec(data[2] & 0x3f)  #Need to change this if 12 hour am/pm
            self.dayOfWeek = self.bcdToDec(data[3])
            self.dayOfMonth = self.bcdToDec(data[4])
            self.month = self.bcdToDec(data[5])
            self.year = self.bcdToDec(data[6])

            print 'getTime..'

        def fillByHMS(self, _hour,  _minute,  _second):
            self.hour = _hour
            self.minute = _minute
            self.second = _second

            print 'fillByHMS..'

        def fillByYMD(self, _year,  _month,  _day):     
            self.year = _year - 2000
            self.month = _month;
            self.dayOfMonth = _day

            print 'fillByYMD..'

        def fillDayOfWeek(self,  _dow):     
            self.dayOfWeek = _dow

            print 'fillDayOfWeek..'

    if __name__ == "__main__":
        clock = DS1307()
        clock.fillByYMD(2015,3,5)
        clock.fillByHMS(12,42,30)
        clock.fillDayOfWeek(clock.THU)  
        clock.setTime()
        while True:     
            clock.getTime()
            print clock.hour, ":", clock.minute, ":", \
                    clock.second, " ", clock.dayOfMonth, "/", \
                    clock.month, "/", clock.year,"  ", "weekday", \
                    ":", clock.dayOfWeek            
            time.sleep(1)
```

 Thực hiện các lệnh dưới đây để sử dụng cảm biến này

```bash
    sudo python grove_rtc.py
```

Đây là kết quả

![](https://github.com/SeeedDocument/Grove-RTC/raw/master/img/rpi_display2.jpg)


## Nguồn


- **[Eagle]** [Grove-RTC in Eagle format](https://raw.githubusercontent.com/SeeedDocument/Grove-RTC/master/res/Real_Time_Clock.zip)
- **[PDF]** [Grove-RTC Schematic in PDF format](https://github.com/SeeedDocument/Grove-RTC/raw/master/res/Grove%20-%20RTC%20v1.1%20Sch.pdf)
- **[PDF]** [Grove-RTC PCB in PDF format](https://github.com/SeeedDocument/Grove-RTC/raw/master/res/Grove%20-%20RTC%20v1.1%20PCB.pdf)
- **[Library]**[Github repository for RTC](https://github.com/Seeed-Studio/RTC_DS1307/archive/master.zip)
- **[Datasheet]** [DS1307 Datasheet](https://raw.githubusercontent.com/SeeedDocument/Grove-RTC/master/res/DS1307.pdf)

## Dự án

**Sử dụng đồng hồ thời gian thực với Arduino**: Bạn đã bao giờ muốn thực hiện một dự án kích hoạt theo lịch trình chưa? Sử dụng Đồng hồ thời gian thực (RTC) là một cách tuyệt vời để làm điều đó!

<iframe frameborder='0' height='327.5' scrolling='no' src='https://www.hackster.io/robotgeek-projects-team/using-a-real-time-clock-with-arduino-6b3896/embed' width='350'></iframe>

**Đồng hồ nhiều màu sắc**: Đồng hồ hiển thị mức năng lượng của bạn và chào đón bạn khi bạn đến gần

<iframe frameborder='0' height='327.5' scrolling='no' src='https://www.hackster.io/zou-wei/colorful-clock-4cea6b/embed' width='350'></iframe>

## Hỗ trợ kỹ thuật
Vui lòng gửi bất kỳ vấn đề kỹ thuật vào [diễn đàn](http://forum.seeedstudio.com/) của chúng tôi.
<br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>