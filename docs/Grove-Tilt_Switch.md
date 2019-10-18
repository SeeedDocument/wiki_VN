---
name: Grove - Tilt Switch
category: Sensor
bzurl: https://seeedstudio.com/Grove-Tilt-Switch-p-771.html
oldwikiname: Grove_-_Tilt_Switch
prodimagename: Tilt1.jpg
bzprodimageurl: http://statics3.seeedstudio.com/images/product/gbtlt.jpg
surveyurl: https://www.research.net/r/Grove-Tilt_Switch
sku: 101020025
tags: grove_digital, io_3v3, io_5v, plat_duino, plat_pi, plat_bbg
---

![](https://raw.githubusercontent.com/SeeedDocument/Grove-Tilt_Switch/master/img/Tilt1.jpg)

Grove-Tilt Switch tương đương với một nút và được sử dụng làm đầu vào kỹ thuật số. Bên trong công tắc nghiêng là một cặp bóng tiếp xúc với các chân khi vỏ thẳng đứng. Nghiêng trường hợp và các quả bóng không chạm vào, do đó không tạo ra kết nối. Nó được nối với dòng SIG, NC không được sử dụng trên Grove này.

[![](https://raw.githubusercontent.com/SeeedDocument/common/master/Get_One_Now_Banner.png)](https://www.seeedstudio.com/Grove-Tilt-Switch-p-771.html)

Đặc điểm
--------

-   Giao diện Grove
-   Dễ sử dụng
-   Module Grove đơn giản

!!!Mẹo
    Thông tin chi tiết về các module Grove vui lòng tham khảo [Hệ thống Grove](http://wiki.seeedstudio.com/Grove_System/)
    
Các thông số kỹ thuật
--------------

<table border="1" cellspacing="0" width="80%">
<tr>
<th scope="col">
Item
</th>
<th scope="col">
Nhỏ nhất
</th>
<th scope="col">
Điển hình
</th>
<th scope="col">
Lớn nhất
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
3
</td>
<td>
5.0
</td>
<td>
5.25
</td>
<td>
V
</td>
</tr>
<tr align="center">
<th scope="row">
Góc kết nối
</th>
<td colspan="3">
10° ~170°
</td>
<td>
-
</td>
</tr>
<tr align="center">
<th scope="row">
Góc mất kết nối
</th>
<td colspan="3">
190° ~350°
</td>
<td>
-
</td>
</tr>
<tr align="center">
<th scope="row">
Độ bền điện
</th>
<td colspan="3">
100,000
</td>
<td>
Cycle
</td>
</tr>
</table>

Các nền tảng được hỗ trợ
-------------------

| Arduino                                                                                             | Raspberry Pi                                                                                             | BeagleBone                                                                                      | Wio                                                                                               | LinkIt ONE                                                                                         |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/arduino_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/raspberry_pi_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/bbg_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/wio_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/linkit_logo_n.jpg) |

!!!Chú ý
    Các nền tảng được đề cập ở trên được hỗ trợ như chỉ dẫn của phần mềm của module hoặc khả năng tương thích về mặt lý thuyết. Chúng tôi chỉ cung cấp thư viện phần mềm hoặc các ví dụ cho nền tảng Arduino trong hầu hết các trường hợp. Không thể cung cấp thư viện phần mềm / mã demo cho tất cả các nền tảng MCU. Do đó, người dùng phải viết thư viện phần mềm của riêng họ.


## Getting Started

### Đối với Arduino

Chân SIG của Grove - Tilt Switch thông thườn đầu ra THẤP. Khi Tilt Switch thẳng đứng, một cặp bóng bên trong công tắc nghiêng sẽ tiếp xúc với các chân và chân SIG sẽ ra ở mức CAO.

Sketch sau đây cho thấy một ứng dụng đơn giản là sử dụng Tilt Switch và Grove - Button để điều khiển đèn led.


-   Như hình ảnh sau đây cho thấy, Tilt Switch được kết nối với cổng kỹ thuật số 5 của Grove - Base Shield và Grove-Button với cổng số 7. Đèn LED được kết nối với cổng số 1. Việc cài đặt phần cứng như sau:

![](https://raw.githubusercontent.com/SeeedDocument/Grove-Tilt_Switch/master/img/Digitalv1.0b.jpg)

-   Sao chép và dán mã dưới đây vào sketch mới.

```
void setup()
{
    pinMode(1, OUTPUT);
    pinMode(5, INPUT);
    pinMode(7, INPUT);
}

void loop()
{

    if (digitalRead(5)==HIGH)
    {
        digitalWrite(1, HIGH);
        delay(100);
        digitalWrite(1, LOW);
    }

    if (digitalRead(7)==HIGH)
    {
        digitalWrite(1, HIGH);
        delay(200);
        digitalWrite(1, LOW);
    }

}
```

-   Tải code lên.
-   Sau đó, đèn LED sẽ sáng khi bạn nhấn nút hoặc kích hoạt công tắc nghiêng. Thử!

### Đối với Codecraft

#### Phần cứng

**Bước 1.** Kết nối Grove - Tilt Switch tới cổng D5, kết nối Grove - Button và Grove - Red LED tới cổng D7 và D2 của Base Shield.

**Bước 2.** Cắm Base Shield vào Seeeduino/Arduino của bạn.

**Bước 3.** Kết nối Seeeduino/Arduino tới PC qua cáp USB.

#### Phần mềm

**Bước 1.** Mở [Codecraft](https://ide.chmakered.com/), thêm hỗ trợ Arduino và kéo một lệnh chính vào vùng làm việc.

!!!Chú ý
   Nếu đây là lần đầu tiên bạn sử dụng Codecraft, hãy xem thêm [Hướng dẫn sử dụng Codecraft bằng Arduino](http://wiki.seeedstudio.com/Guide_for_Codecraft_using_Arduino/).

**Step 2.** Kéo các khối như hình dưới đây hoặc mở tệp cdc có thể được tải xuống ở cuối trang này.

![cc](https://raw.githubusercontent.com/SeeedDocument/Grove-Tilt_Switch/master/img/cc_Tilt_Switch.png)

Tải chương trình lên Arduino / Seeeduino của bạn.

!!!Kết quả
    Khi mã được tải lên, nghiêng công tắc nghiêng hoặc nhấn nút, đèn LED sẽ sáng.

### Đối với Raspberry Pi (Với Grove Base Hat cho Raspberry Pi)

#### Phần cứng

- **Bước 1**. Các thứ được sử dụng trong dự án:

| Raspberry pi | Grove Base Hat for RasPi| Grove - Tilt Switch |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Base_Hat_for_Raspberry_Pi/raw/master/img/thumbnail.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Tilt_Switch/raw/master/img/thumbnail.jpg)|
|[Get ONE Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Base-Hat-for-Raspberry-Pi-p-3186.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Tilt-Switch-p-771.html)|

- **Step 2**. Cắm Grove Base Hat vào Raspberry.
- **Step 3**. Kết nối tilt switch tới cổng 12 của Base Hat.
- **Step 4**. Kết nối the Raspberry Pi ới PC qua cáp USB.


![](https://github.com/SeeedDocument/Grove-Tilt_Switch/raw/master/img/Tilt_Hat.jpg)

!!! Chú ý
    Đối với bước 3, bạn có thể kết nối ultrasonic ranger với **bất kỳ Cổng GPIO nào** nhưng đảm bảo bạn thay đổi lệnh với số cổng tương ứng.



#### Phần mềm

- **Step 1**. Theo dõi [Cài đặt phần mềm](http://wiki.seeedstudio.com/Grove_Base_Hat_for_Raspberry_Pi/#installation) để cấu hình môi trường phát triển.
- **Step 2**. Tải xuống tệp nguồn bằng cách nhân bản thư viện grove.py.  

```
cd ~
git clone https://github.com/Seeed-Studio/grove.py

```

- **Step 3**. Thực hiện các lệnh dưới đây để chạy mã.

```
cd grove.py/grove
python grove_tilt_switch.py 12

```

Dưới đây là code grove_tilt_switch.py.

```python

import time
from grove.gpio import GPIO


class GroveTiltSwitch(GPIO):
    def __init__(self, pin):
        super(GroveTiltSwitch, self).__init__(pin, GPIO.IN)
        self._on_trigger = None
        self._on_release = None

    @property
    def on_trigger(self):
        return self._on_trigger

    @on_trigger.setter
    def on_trigger(self, callback):
        if not callable(callback):
            return

        if self.on_event is None:
            self.on_event = self._handle_event

        self._on_trigger = callback

    @property
    def on_release(self):
        return self._on_release

    @on_release.setter
    def on_release(self, callback):
        if not callable(callback):
            return

        if self.on_event is None:
            self.on_event = self._handle_event

        self._on_release = callback

    def _handle_event(self, pin, value):

        if value:
            if callable(self._on_trigger):
                self._on_trigger()
        else:
            if callable(self._on_release):
                self._on_release()

Grove = GroveTiltSwitch


def main():
    import sys

    if len(sys.argv) < 2:
        print('Usage: {} pin'.format(sys.argv[0]))
        sys.exit(1)

    swicth = GroveTiltSwitch(int(sys.argv[1]))

    def on_trigger():
        print('Triggered')
    def on_release():
        print("Released.")

    swicth.on_trigger = on_trigger
    swicth.on_release = on_release

    while True:
        time.sleep(1)


if __name__ == '__main__':
    main()


```

!!!Kết quả
    Nếu mọi thứ suôn sẻ, bạn sẽ thấy kết quả sau khi bạn chạm vào công tắc nghiêng.

```python

pi@raspberrypi:~/grove.py/grove $ python grove_tilt_switch.py 12
Triggered
Released.
Triggered
^CTraceback (most recent call last):
  File "grove_tilt_switch.py", line 106, in <module>
    main()
  File "grove_tilt_switch.py", line 102, in main
    time.sleep(1)
KeyboardInterrupt

```

Bạn có thể thoát chương trình này đơn giản bằng cách nhấn ++ ctrl + c ++.




### Đối với Raspberry Pi (with GrovePi_Plus)


### Với Raspberry Pi

1.Bạn nên có Raspberry Pi và Grovepi hoặc Grovepi +. 

2.Bạn đã hoàn tất việc cấu hình môi trường phát triển, nếu không, hãy làm theo [tại đây] (/GrovePi_Plus).

3.Kết nối

-   Cắm Tilt_Switch vào ổ cắm Grovepi D3 bằng cách sử dụng cáp grove.

4.Điều hướng đến thư mục của các bản demo:
```
       cd yourpath/GrovePi/Software/Python/
```
-   Để thấy code
```
    nano grovepi_tilt_switch.py   # "Ctrl+x" to exit #
```
```
    import time
    import grovepi

    # Connect the Grove Tilt Switch to digital port D3
    # SIG,NC,VCC,GND
    tilt_switch = 3

    grovepi.pinMode(tilt_switch,"INPUT")

    while True:
        try:
            print grovepi.digitalRead(tilt_switch)
            time.sleep(.5)

        except IOError:
            print "Error"
```

5.Chạy demo.

```
    sudo python grove_tilt_switch.py
```

6.Kết quả: Đặt cảm biến thẳng đứng ở một bên, chân SIG sẽ ra ở mức CAO.

![](https://raw.githubusercontent.com/SeeedDocument/Grove-Tilt_Switch/master/img/Grovepi_tilt_Switch_00.png)



Tài liệu tham khảo
---------

Góc vận hành của Grove-Tilt Switch như hình dưới đây:

![](https://raw.githubusercontent.com/SeeedDocument/Grove-Tilt_Switch/master/img/Tilt_Switch_Operate.jpg)

<div class="admonition note">
<p class="admonition-title">Chú ý</p>
Dấu J1 trên Grove là thiết bị đầu cuối tham chiếu.
</div>



Nguồn
---------

-   [Grove - Tilt Switch v1.0 Eagle File](https://raw.githubusercontent.com/SeeedDocument/Grove-Tilt_Switch/master/res/Grove-Tilt_Switch_v1.0_Source_File.zip)
-   [Grove - Tilt Switch v1.1 PDF File](https://raw.githubusercontent.com/SeeedDocument/Grove-Tilt_Switch/master/res/Grove-Tilt_Switch_v1.1_PDF_File.pdf)
-   [Grove - Tilt Switch v1.1 Eagle File](https://raw.githubusercontent.com/SeeedDocument/Grove-Tilt_Switch/master/res/Grove-Tilt_Switch_v1.1_Eagle_File.zip)
-   [SW200D Datasheet](https://raw.githubusercontent.com/SeeedDocument/Grove-Tilt_Switch/master/res/SW200D_datasheet.pdf)
-   [Codecraft CDC File](https://raw.githubusercontent.com/SeeedDocument/Grove-Tilt_Switch/master/res/Grove_Tilt_Switch_CDC_File.zip)


<!-- This Markdown file was created from http://www.seeedstudio.com/wiki/Grove_-_Tilt_Switch -->

## Hỗ trợ kỹ thuật
Vui lòng gửi bất kỳ vấn đề kỹ thuật vào [diễn đàn](http://forum.seeedstudio.com/) của chúng tôi. <br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>