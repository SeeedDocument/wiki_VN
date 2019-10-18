---
name: Grove-LED Button
category: Acator
bzurl: 
oldwikiname: 
prodimagename:
surveyurl: 
sku: 111020044,111020045,111020046
tags: 2-链接 
---


![](https://github.com/SeeedDocument/Grove-Red_LED_Button/raw/master/img/main.jpg)


Grove - LED Button gồm Grove - Yellow Button, Grove - Blue LED Button và Grove - Red LED Button. Nút này ổn định và đáng tin cậy với tuổi thọ 100 000 lần.
Với đèn LED tích hợp, bạn có thể áp dụng nó cho nhiều dự án thú vị, thực sự hữu ích khi sử dụng đèn LED để hiển thị trạng thái của nút. Chúng tôi sử dụng MOSFET N-Channel chất lượng cao để điều khiển đèn LED để đảm bảo tốc độ quét cao và mức tiêu thụ thấp. Tất cả, bạn có muốn một số nút đáng tin cậy không? Bạn đi đây ...



<p style=":center"><a href="https://www.seeedstudio.com/Grove-Yellow-LED-Button-p-3101.html" target="_blank"><img src="https://github.com/SeeedDocument/Grove-Red_LED_Button/raw/master/img/Y.png" height="48" width="300" /></a></p>
<p style=":center"><a href="https://www.seeedstudio.com/Grove-Blue-LED-Button-p-3104.html" target="_blank"><img src="https://github.com/SeeedDocument/Grove-Red_LED_Button/raw/master/img/B.png" height="48" width="300" /></a></p>
<p style=":center"><a href="https://www.seeedstudio.com/Grove-Red-LED-Button-p-3096.html" target="_blank"><img src="https://github.com/SeeedDocument/Grove-Red_LED_Button/raw/master/img/R.png"  height="48" width="300" /></a></p>

## Phiên bản

| Phiên bản sản phẩm  | Thay đổi                                                                                               | Ngày phát hành |
|------------------|-------------------------------------------------------------------------------------------------------|---------------|
| Grove-LED Button |  Ban đầu                                                                                               | 06/2018      |


## Đặc tính

- Tuổi thọ hoạt động lâu
- Dễ sử dụng
- Giao diện số Grove



## Các thông số kỹ thuật

|Item|Giá trị|
|---|---|
|Điện áp hoạt động|3.3V/5V|
|Tuổi thọ hoạt động không tải|100 000 times|
|Dòng LED định mức|50mA|
|Điện trở ấn^1^|<100mΩ|
|Điện trở nhả^2^|>100MΩ|
|Kích thước|D: 40mm R: 20mm C: 13mm| 
|Khối lượng|4.3g|
|Kích thước đóng gói|D: 140mm R: 90mm C: 10mm|
|Tổng trọng lượng|11g|



!!!Lời khuyên
         1,2- Nếu bạn muốn đo điện trở, vui lòng lấy nắp khóa ra khỏi mạch. Nếu không, bạn sẽ nhận được giá trị của điện trở tương đương của mạch thay vì điện trở thực sự của nắp khóa.



## Tổng quan phần cứng


### Sơ đồ chân


![](https://github.com/SeeedDocument/Grove-Red_LED_Button/raw/master/img/pin_map.jpg)


### Sơ đồ nguyên lý

![](https://github.com/SeeedDocument/Grove-Red_LED_Button/raw/master/img/schematic.jpg)


**SIG1** là tín hiệu điều khiển LED, giá trị mặc định thấp, do đó MOSFET kênh N bị tắt, đèn LED cũng tắt. Khi SIG1 trở nên cao, MOSFE N-Channel bật và đèn LED sáng.

**SIG2** kết nối với pin nút. Với điện trở kéo lên, giá trị mặc định của **SIG2** là cao. Khi bạn nhấn nút, điện áp được kéo xuống thấp, **SIG2** trở thành mức thấp.




## Các nền tảng được hỗ trợ

| Arduino                                                                                             | Raspberry Pi                                                                                             | BeagleBone                                                                                      | Wio                                                                                               | LinkIt ONE                                                                                         |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/arduino_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/raspberry_pi_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/bbg_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/wio_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/linkit_logo.jpg) |




## Getting Started

!!!Lời khuyên
         Trong phần này, chúng tôi sử dụng Nút đèn LED màu đỏ - Grove làm ví dụ. Các phần sau đây cũng áp dụng cho Vàng và Xanh.


### Đối với Arduino

#### Phần cứng

**Vật liệu thiết yếu**


| Seeeduino V4.2 | Base Shield| Grove- Red LED Button |
|--------------|-------------|-----------------|
|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_1.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_4.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Red_LED_Button/raw/master/img/IMG_0068a.jpg)|
|<a href="http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html" target="_blank">Get One Now</a>|<a href="https://www.seeedstudio.com/Base-Shield-V2-p-1378.html" target="_blank">Get One Now</a>|<a href="https://www.seeedstudio.com/Grove-Red-LED-Button-p-3096.html" target="_blank">Get One Now</a>|



- **Bước 1.** Nối Grove- Red LED Button tới cổng **D3** của Grove-Base Shield.

- **Bước 2.** Cắm Grove - Base Shield vào Seeeduino.

- **Bước 3.** Kết nối Seeeduino tới PC qua một cáp USB.


![](https://github.com/SeeedDocument/Grove-Red_LED_Button/raw/master/img/red%20LED.jpg)


!!!Chú ý
Nếu chúng tôi không có Grove Base Shield,chúng tôi cũng có thể kết nối trực tiếp module này tới Seeeduino như dưới đây.


| Seeeduino     |  Grove- Red LED Button           |
|---------------|-------------------------|
| 5V            | Đỏ                     |
| GND           | Đen                   |
| SIG2           | Trắng                  |
| SIG1          | Vàng                  |




#### Phần mềm

!!!Chú thích
    Nếu đây là lần đầu tiên bạn làm việc với Arduino, chúng tôi chắc chắn khuyên bạn nên xem [Bắt đầu với Arduino](http://wiki.seeedstudio.com/Getting_Started_with_Arduino/) trước khi bắt đầu.


- **Bước 1.** Mở Arduino IDE và tạo một tệp mới, sau đó sao chép đoạn mã sau vào tệp mới.

```C++
#include "Arduino.h"

//1: toggle mode, 2: follow mode
#define LED_MODE   1

const int ledPin = 3;      // the number of the LED pin, D3
const int buttonPin = 4;    // the number of the pushbutton pin, D4
const boolean breathMode = true;  // if or not the led lights as breath mode when it's on

// Variables will change:
int ledState = LOW;         // the current state of the output pin
int ledFadeValue = 0;
int ledFadeStep = 5;
int ledFadeInterval = 20;   //milliseconds
int buttonState;             // the current reading from the input pin
int lastButtonState = HIGH;   // the previous reading from the input pin

unsigned long lastDebounceTime = 0;  // the last time the output pin was toggled
unsigned long debounceDelay = 50;    // the debounce time; increase if the output flickers
unsigned long lastLedFadeTime = 0;

void setup() {
  pinMode(buttonPin, INPUT);
  pinMode(ledPin, OUTPUT);
  digitalWrite(ledPin, ledState);
}

void loop() {
  int reading = digitalRead(buttonPin);

  // If the switch changed, due to noise or pressing:
  if (reading != lastButtonState) {
    // reset the debouncing timer
    lastDebounceTime = millis();
  }

  if ((millis() - lastDebounceTime) > debounceDelay) {
    // whatever the reading is at, it's been there for longer
    // than the debounce delay, so take it as the actual current state:

    // if the button state has changed:
    if (reading != buttonState) {
      buttonState = reading;

#if LED_MODE == 1
      if (buttonState == LOW) {  //button is pressed
          ledState = !ledState;
          ledFadeValue = 0;
          lastLedFadeTime = millis();
      }
#else
      if (buttonState == LOW) {  //button is pressed
        ledState = HIGH;
        ledFadeValue = 0;
        lastLedFadeTime = millis();
      } else {                   //button is released
        ledState = LOW;
      }
#endif
    }
  }

  // set the LED:
  if (breathMode && ledState != LOW) {
    if (millis() - lastLedFadeTime > ledFadeInterval) {
      lastLedFadeTime = millis();
      analogWrite(ledPin, ledFadeValue);
      ledFadeValue += ledFadeStep;
      if (ledFadeValue > 255){
        ledFadeValue = 255 - ledFadeStep;
        ledFadeStep = -ledFadeStep;
      } else if (ledFadeValue < 0) {
        ledFadeValue = 0;
        ledFadeStep = -ledFadeStep;
      }
    }
  } else {
    digitalWrite(ledPin, ledState);
  }

  lastButtonState = reading;
}

```

!!!Mẹo
     Trong bản demo này, chúng tôi chọn chế độ 1 là chế độ chuyển đổi, bạn có thể thay đổi dòng 4 <mark>#define LED_MODE   1</mark> thành <mark>#define LED_MODE   2</mark> để sử dụng chế độ theo dõi.

- **Bước 2.** Tải lên bản demo. Nếu bạn không biết cách tải lên mã, vui lòng kiểm tra [Cách tải lên mã](http://wiki.seeedstudio.com/Upload_Code/).

- **Bước 3.** Bây giờ, hãy thử nhấn nút bạn, bạn sẽ thấy đèn LED bật với hiệu ứng tắt / tắt dần.

Nó sẽ giống như:

<p style=":center"><img src="https://github.com/SeeedDocument/Grove-Red_LED_Button/raw/master/img/result.gif"  /></p>



### Đối với Raspberry Pi

#### Phần cứng

- **Bước 1**. Chuẩn bị những thứ dưới đây:

| Raspberry pi | Grove Base Hat for RasPi| Grove - Red LED Button|
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Base_Hat_for_Raspberry_Pi/raw/master/img/thumbnail.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Red_LED_Button/raw/master/img/IMG_0068a.jpg)|
|[Get ONE Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Base-Hat-for-Raspberry-Pi-p-3186.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Red-LED-Button-p-3096.html)|

- **Step 2**. Cắm Grove Base Hat vào Raspberry.
- **Step 3**. Kết nối nút ấn LED đỏ tới cổng D5 của Base Hat.
- **Step 4**. Kết nối Raspberry Pi tới PC qua cáp USB.

![](https://github.com/SeeedDocument/Grove-Red_LED_Button/raw/master/img/LED_Hat.jpg)

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
python grove_ryb_led_button.py 5

```

Dưới đây là mã grove_ryb_led_button.py.

```python

import time
from grove.button import Button
from grove.factory import Factory

class GroveLedButton(object):
    def __init__(self, pin):
        # High = light on
        self.__led = Factory.getOneLed("GPIO-HIGH", pin)
        # Low = pressed
        self.__btn = Factory.getButton("GPIO-LOW", pin + 1)
        self.__on_event = None
        self.__btn.on_event(self, GroveLedButton.__handle_event)

    @property
    def on_event(self):
        return self.__on_event

    @on_event.setter
    def on_event(self, callback):
        if not callable(callback):
            return
        self.__on_event = callback

    def __handle_event(self, evt):
        # print("event index:{} event:{} pressed:{}".format(evt['index'], evt['code'], evt['presesed']))
        if callable(self.__on_event):
            self.__on_event(evt['index'], evt['code'], evt['time'])
            return

        self.__led.brightness = self.__led.MAX_BRIGHT
        event = evt['code']
        if event & Button.EV_SINGLE_CLICK:
            self.__led.light(True)
            print("turn on  LED")
        elif event & Button.EV_DOUBLE_CLICK:
            self.__led.blink()
            print("blink    LED")
        elif event & Button.EV_LONG_PRESS:
            self.__led.light(False)
            print("turn off LED")


Grove = GroveLedButton

def main():
    from grove.helper import SlotHelper
    sh = SlotHelper(SlotHelper.GPIO)
    pin = sh.argv2pin()

    ledbtn = GroveLedButton(pin)

    # remove ''' pairs below to begin your experiment
    '''
    # define a customized event handle your self
    def cust_on_event(index, event, tm):
        print("event with code {}, time {}".format(event, tm))

    ledbtn.on_event = cust_on_event
    '''
    while True:
        time.sleep(1)


if __name__ == '__main__':
    main()


```

!!!Kết quả
  Nếu mọi thứ suôn sẻ, bạn sẽ có thể thấy đèn LED bật nếu bạn nhấn và tắt nếu bạn nhấn lâu. Nếu bạn nhấp đúp vào nút LED, đèn LED sẽ nhấp nháy.

```python

pi@raspberrypi:~/grove.py/grove $ python grove_ryb_led_button.py 5
Hat Name = 'Grove Base Hat RPi'
turn on  LED
turn on  LED
blink    LED
turn on  LED
turn off LED
^CTraceback (most recent call last):
  File "grove_ryb_led_button.py", line 101, in <module>
    main()
  File "grove_ryb_led_button.py", line 97, in main
    time.sleep(1)
KeyboardInterrupt

```


Bạn có thể thoát chương trình này đơn giản bằng cách nhấn ++ ctrl + c ++.



## Nguồn

- **[Zip]** [Grove-LED Button Eagle file](https://github.com/SeeedDocument/Grove-Red_LED_Button/raw/master/res/Grove-Red_LED_Button.zip)


## Hỗ trợ kỹ thuật
Vui lòng gửi bất kỳ vấn đề kỹ thuật vào [diễn đàn](http://forum.seeedstudio.com/) của chúng tôi. <br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>