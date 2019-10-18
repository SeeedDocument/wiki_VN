---
name: Grove - RGB LED Stick (10 WS2813 Mini)
category: Sensor
bzurl: 
oldwikiname: 
prodimagename:
surveyurl: 
sku: 104020131
tags:
---

![](https://github.com/SeeedDocument/Grove-RGB_LED_Stick-10-WS2813_Mini/raw/master/img/main.jpg)

Chúng tôi đã tích hợp 10 đèn LED RGB đủ màu trên thanh này, chỉ với một chân tín hiệu bạn có thể điều khiển tất cả 10 đèn LED một cách dễ dàng. Tất cả các đèn LED là WS2813 Mini, đây là một điều khiển thông minh và đèn LED hiệu quả cao.
Hơn nữa, WS2813 hỗ trợ truyền liên tục điểm ngắt tín hiệu, có nghĩa là bạn có thể tiếp tục sử dụng các đèn led khác với một đèn led bị hỏng.

Bạn có thể sử dụng cây gậy nhỏ này tạo ra hàng trăm ngàn hiệu ứng ánh sáng, chúng tôi hy vọng nó sẽ mang lại cho bạn nhiều niềm vui hơn.


<p style=":center"><a href="https://www.seeedstudio.com/Grove-RGB-LED-Stick-10-WS2813-Min-p-3226.html" target="_blank"><img src="https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/300px-Get_One_Now_Banner-ragular.png" /></a></p>

## Phiên bản

| Phiên bản sản phẩm  | Thay đổi                                                                                               | Ngày phát hành |
|------------------|-------------------------------------------------------------------------------------------------------|---------------|
| Grove - RGB LED Stick (10 WS2813 Mini) | Ban đầu                                                                                               | 11/2018      |

## Đặc tính

- IC WS2813B, đèn LED 3535
- Bảo vệ kết nối ngược thông minh.
- Các mức độ màu xám của mỗi pixel là 256, đạt được màn hình đầy đủ màu 256 * 256 * 256 = 16777216.
- Tần số làm mới đạt tới 2KHz.
- Giao diện tầng nối tiếp, nhận và giải mã dữ liệu phụ thuộc vào chỉ một đường tín hiệu.
- Phiên bản dây tín hiệu kép, điểm ngắt tín hiệu truyền liên tục.


### Tín hiệu truyền liên tục điểm ngắt

![](https://github.com/SeeedDocument/Outsourcing/raw/master/104020108/img/LED_RFBP.jpg)

Miễn là không có hai hoặc nhiều đèn LED liền kề bị hỏng, các đèn LED còn lại sẽ có thể hoạt động bình thường.



## Đặc điểm kỹ thuật

|Item|Value|
|---|---|
|Điện áp hoạt động|3.3V / 5V|
|Nhiệt độ hoạt động|-25℃ ~ +85℃|
|Nhiệt độ lưu trữ|-40℃ ~ +105℃|
|Dòng không đổi kênh RGB|16mA|
|Giao diện|Số|
|Kích thước|Dài: 80mm Rộng: 10mm Cao: 10mm| 
|Cân nặng|3.7g|
|Kích thước đóng gói|Dài: 150mm Rộng: 100mm Cao: 25mm|
|Tổng trọng lượng|13g|


## Các ứng dụng tiêu biểu
 

- Trang trí giáng sinh
- Chiếu sáng
- Đồ chơi


## Tổng quan về phần cứng

### Chân ra

![](https://github.com/SeeedDocument/Grove-RGB_LED_Stick-10-WS2813_Mini/raw/master/img/pin_out.jpg)



## Nền tảng được hỗ trợ

| Arduino                                                                                             | Raspberry Pi                                                                                             | BeagleBone                                                                                      | Wio                                                                                               | LinkIt ONE                                                                                         |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/arduino_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/raspberry_pi_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/bbg_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/wio_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/linkit_logo_n.jpg) |


!!!Chú ý
    Các nền tảng được đề cập ở trên được hỗ trợ như chỉ dẫn của phần mềm của module hoặc khả năng tương thích về mặt lý thuyết. Chúng tôi chỉ cung cấp thư viện phần mềm hoặc các ví dụ cho nền tảng Arduino trong hầu hết các trường hợp. Không thể cung cấp thư viện phần mềm / mã demo cho tất cả các nền tảng MCU. Do đó, người dùng phải viết thư viện phần mềm của riêng họ.

## Getting Started


### Đối với Arduino


#### Phần cứng

**Vật liệu thiết yếu**

| Seeeduino V4.2 | Base Shield | Grove - RGB LED Stick (10 WS2813 Mini) |
|--------------|-------------|-----------------|
|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_1.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_4.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-RGB_LED_Stick-10-WS2813_Mini/raw/master/img/thumbnail.jpg)|
|<a href="http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html" target="_blank">Get One Now</a>|<a href="https://www.seeedstudio.com/Base-Shield-V2-p-1378.html" target="_blank">Get One Now</a>|<a href="https://www.seeedstudio.com/Grove-RGB-LED-Stick-10-WS2813-Min-p-3226.html" target="_blank">Get One Now</a>|


!!!chú ý
    **1** Vui lòng cắm cáp USB nhẹ nhàng, nếu không bạn có thể làm hỏng cổng. Vui lòng sử dụng cáp USB có 4 dây bên trong, cáp 2 dây không thể truyền dữ liệu. Nếu bạn không chắc chắn về dây bạn có, bạn có thể nhấp vào [đây](https://www.seeedstudio.com/Micro-USB-Cable-48cm-p-1475.html) để mua.
    
    **2** Each Grove module comes with a Grove cable when you buy. In case you lose the Grove cable, you can click [here](https://www.seeedstudio.com/Grove-Universal-4-Pin-Buckled-20cm-Cable-%285-PCs-pack%29-p-936.html) to buy.


!!!Quan trọng
    **1**. Nếu bạn sử dụng Arduino UNO làm bo mạch chủ, bạn nên sử dụng nguồn điện DC. Mặt khác, độ gợn tối đa của VCC có thể vượt quá 100mV. Nếu bạn sử dụng Seeeduino V4.2 làm bo mạch chủ, bạn không cần kết nối nguồn DC.

    **2**. Trao đổi nóng không được hỗ trợ.


- **Step 1.** Kết nối Grove - RGB LED Stick (10 WS2813 Mini) với cổng **D6** của Grove-Base Shield.

- **Step 2.** Cắm Grove - Base Shield vào Seeeduino.

- **Step 3.** Kết nối Seeeduino với PC thông qua cáp USB.


![](https://github.com/SeeedDocument/Grove-RGB_LED_Stick-10-WS2813_Mini/raw/master/img/connect.jpg)

!!!Chú ý
Nếu chúng tôi không có Grove Base Shield, chúng tôi cũng có thể kết nối trực tiếp module này tới Seeeduino như dưới đây.


| Seeeduino      |  Grove Cable       | Grove - RGB LED Stick (10 WS2813 Mini) |
|--------------- |--------------------|-----|
| GND            | Đem              | GND |
| 5V or 3.3V     | Đỏ                | VCC |
| Không kết nối          | Trắng              | NC |
| D6            | Vàng             | SIG |



#### Phần mềm

!!!Chú ý
        Nếu đây là lần đầu tiên bạn làm việc với Arduino, chúng tôi thực sự khuyên bạn nên xem [Bắt đầu với Arduino] (http://wiki.seeedstudio.com/Getting_Started_with_Arduino/) trước khi bắt đầu.


- **Bước 1.** Tải xuống [Led_Strip](https://github.com/Seeed-Studio/Seeed_Led_Strip) Library từ Github.

- **Bước 2.** Tham khảo [How to install library](http://wiki.seeedstudio.com/How_to_install_Arduino_Library) để cài đặt thư viện cho Arduino.
- **Bước 3.** Khởi động lại Arduino IDE. Mở ví dụ, bạn có thể mở nó theo ba cách sau:
    1. Mở nó trực tiếp trong Arduino IDE thông qua đường dẫn **File --> Examples --> Adafruit_Neopixel --> simple**. 
    ![](https://github.com/SeeedDocument/Grove-RGB_LED_Stick-10-WS2813_Mini/raw/master/img/path1.jpg)
    
    2. Mở nó trong máy tính của bạn bằng cách nhấp vào **Simple.ino** mà bạn có thể tìm thấy trong thư mục **XXXX\Arduino\libraries\Seeed_Led_Strip-master\examples\simple**, **XXXX** là vị trí bạn đã cài đặt Arduino IDE.
    ![](https://github.com/SeeedDocument/Grove-RGB_LED_Stick-10-WS2813_Mini/raw/master/img/path2.jpg)
    
    3. Hoặc, bạn chỉ cần nhấp vào biểu tượng ![](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/copy.jpg) ở góc trên bên phải của khối mã để sao chép đoạn mã sau vào bản phác thảo mới trong Arduino IDE.

```C++
// NeoPixel Ring simple sketch (c) 2013 Shae Erisson
// released under the GPLv3 license to match the rest of the AdaFruit NeoPixel library

#include "Adafruit_NeoPixel.h"
#ifdef __AVR__
  #include <avr/power.h>
#endif

// Which pin on the Arduino is connected to the NeoPixels?
// On a Trinket or Gemma we suggest changing this to 1
#define PIN            6

// How many NeoPixels are attached to the Arduino?
#define NUMPIXELS      10

// When we setup the NeoPixel library, we tell it how many pixels, and which pin to use to send signals.
// Note that for older NeoPixel strips you might need to change the third parameter--see the strandtest
// example for more information on possible values.
Adafruit_NeoPixel pixels = Adafruit_NeoPixel(NUMPIXELS, PIN, NEO_GRB + NEO_KHZ800);

int delayval = 500; // delay for half a second

void setup() {
  // This is for Trinket 5V 16MHz, you can remove these three lines if you are not using a Trinket
#if defined (__AVR_ATtiny85__)
  if (F_CPU == 16000000) clock_prescale_set(clock_div_1);
#endif
  // End of trinket special code
  pixels.setBrightness(255);
  pixels.begin(); // This initializes the NeoPixel library.
}

void loop() {

  // For a set of NeoPixels the first NeoPixel is 0, second is 1, all the way up to the count of pixels minus one.

  for(int i=0;i<NUMPIXELS;i++){

    // pixels.Color takes RGB values, from 0,0,0 up to 255,255,255
    pixels.setPixelColor(i, pixels.Color(0,150,0)); // Moderately bright green color.

    pixels.show(); // This sends the updated pixel color to the hardware.

    delay(delayval); // Delay for a period of time (in milliseconds).

  }
}
```

!!!Chú ý
         Các tập tin thư viện có thể được cập nhật. Mã này có thể không áp dụng được cho tệp thư viện đã cập nhật, vì vậy chúng tôi khuyên bạn nên sử dụng hai phương pháp đầu tiên.


- **Step 4.** Tải lên bản demo. Nếu bạn không biết cách tải lên mã, vui lòng kiểm tra [Cách tải lên mã](http://wiki.seeedstudio.com/Upload_Code/).



!!!Kết quả
  Nếu mọi thứ đều ổn, bây giờ bạn có thể thấy dải đèn LED sáng:


![](https://github.com/SeeedDocument/Grove-RGB_LED_Stick-10-WS2813_Mini/raw/master/img/test20181210_162208.gif)


## Nguồn

- **[Zip]** [Grove - RGB LED Stick (10 WS2813 Mini) Eagle Files](https://github.com/SeeedDocument/Grove-RGB_LED_Stick-10-WS2813_Mini/raw/master/res/Grove%20-%20RGB%20LED%20Stick%20(10-WS2813%20Mini).zip)

- **[Zip]** [Led_Strip Library](https://github.com/Seeed-Studio/Seeed_Led_Strip/archive/master.zip)

- **[PDF]** [Datasheet WS2813-Mini](https://github.com/SeeedDocument/Grove-RGB_LED_Stick-10-WS2813_Mini/raw/master/res/WS2813-Mini.pdf)




## Hỗ trợ kỹ thuật

Vui lòng gửi bất kỳ vấn đề kỹ thuật vào [diễn đàn](http://forum.seeedstudio.com/) của chúng tôi. <br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>