---
name: Grove - 16 x 2 LCD
category: Display
bzurl: 
oldwikiname: 
prodimagename:
surveyurl: 
sku: 104020111,104020112,104020113
tags:
---

![](https://github.com/SeeedDocument/Grove-16x2_LCD_Series/raw/master/img/main.jpg)


[Grove - LCD RGB Backlight](http://wiki.seeedstudio.com/Grove-LCD_RGB_Backlight/) đã được đón nhận kể từ khi thành lập. Dựa trên phản hồi của khách hàng, giờ đây, chúng tôi mang đến công cụ phái sinh đèn nền đơn sắc hiệu quả hơn cho bạn, tức là, 

The Grove - 16 x 2 LCD (Màu đen nền vàng)  
The Grove - 16 x 2 LCD (Màu đen nền đỏ)  
The Grove - 16 x 2 LCD (Màu trắng nền xanh)  
  
Ngoại trừ đèn nền RGB, ba sản phẩm này gần giống với Đèn nền RGB - LCD RGB, chúng đều rộng 16 ký tự, 2 hàng với đèn nền có độ sáng cao.



<p style=":center"><a href="https://www.seeedstudio.com/Grove-16-x-2-LCD-%28Black-on-Yellow%29-p-3198.html" target="_blank"><img src="https://github.com/SeeedDocument/Grove-16x2_LCD_Series/raw/master/img/Y1.png" height="48" width="300" /></a></p>
<p style=":center"><a href="https://www.seeedstudio.com/Grove-16-x-2-LCD-%28Black-on-Red%29-p-3197.html" target="_blank"><img src="https://github.com/SeeedDocument/Grove-16x2_LCD_Series/raw/master/img/R1.png" height="48" width="300" /></a></p>
<p style=":center"><a href="https://www.seeedstudio.com/Grove-16-x-2-LCD-%28White-on-Blue%29-p-3196.html" target="_blank"><img src="https://github.com/SeeedDocument/Grove-16x2_LCD_Series/raw/master/img/B1.png"  height="48" width="300" /></a></p>


## Đặc tính

- Cấu trúc hiển thị: 16 ký tự * 2 dòng
- Chế độ hiển thị: STN (Vàng xanh)
- Trên mạch MCU
- Giao diện bus I2C
- Hỗ trợ phông chữ tiếng Anh và tiếng Nhật


## Các thông số kỹ thuật

|Item|Giá trị|
|---|---|
|Điện áp hoạt động|3.3V / 5V|
|Nhiệt độ hoạt động|0 to 50℃|
|Nhiệt độ lưu trữ|-10 to 60℃|
|Phương pháp driving|1/16 duty, 1/5 bias|
|Giao diện|I^2^C|
|Địa chỉ I^2^C |0X3E|


## Các ứng dụng điển hình

- Hiển thị nhiệt độ
- Hiển thị thời gian
- Bất kỳ dự án nào cần một màn hình đơn giản



## Tổng quan phần cứng

### Outline

![](https://github.com/SeeedDocument/Grove-16x2_LCD_Series/raw/master/img/outline.jpg)


## Các nền tảng được hỗ trợ

| Arduino                                                                                             | Raspberry Pi                                                                                             | BeagleBone                                                                                      | Wio                                                                                               | LinkIt ONE                                                                                         |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/arduino_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/raspberry_pi_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/bbg_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/wio_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/linkit_logo_n.jpg) |


!!!Chú ý
    Các nền tảng được đề cập ở trên được hỗ trợ như chỉ dẫn của phần mềm của module hoặc khả năng tương thích về mặt lý thuyết. Chúng tôi chỉ cung cấp thư viện phần mềm hoặc các ví dụ cho nền tảng Arduino trong hầu hết các trường hợp. Không thể cung cấp thư viện phần mềm / mã demo cho tất cả các nền tảng MCU. Do đó, người dùng phải viết thư viện phần mềm của riêng họ.





## Getting Started


### Đối với Arduino


#### Phần cứng

**Thiết bị thiết yếu**

| Seeeduino V4.2 | Base Shield|  Grove - 16 x 2 LCD |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/seeeduino_v4.2.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/base_shield.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-16x2_LCD_Series/raw/master/img/perspective.jpg)|
|[Get One Now](http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html)|[Get One Now](https://www.seeedstudio.com/Base-Shield-V2-p-1378.html)|[Get One Now](https://www.seeedstudio.com/Grove-16-x-2-LCD-%28Black-on-Yellow%29-p-3198.html)|


!!!chú ý
    **1**  Vui lòng cắm cáp USB nhẹ nhàng, nếu không bạn có thể làm hỏng cổng. Vui lòng sử dụng cáp USB có 4 dây bên trong, cáp 2 dây không thể truyền dữ liệu. Nếu bạn không chắc chắn về dây bạn có, bạn có thể nhấp vào [tại đây](https://www.seeedstudio.com/Micro-USB-Cable-48cm-p-1475.html) để mua
    
    **2** Mỗi module Grove đi kèm với cáp Grove khi bạn mua. Trong trường hợp bạn mất cáp Grove, bạn có thể nhấp vào [tại đây](https://www.seeedstudio.com/Grove-Universal-4-Pin-Buckled-20cm-Cable-%285-PCs-pack%29-p-936.html) để mua.


- **Bước 1.** Kết nối Grove - 16 x 2 LCD tới cổng **I^2^C** của Grove-Base Shield.

- **Bước 2.** Cắm Grove - Base Shield vào Seeeduino.

- **Bước 3.** Kết nối Seeeduino tới PC qua một cáp USB.


![](https://github.com/SeeedDocument/Grove-16x2_LCD_Series/raw/master/img/connect.jpg)


!!!Chú ý
Nếu chúng tôi không có Grove Base Shield, chúng tôi cũng có thể kết nối trực tiếp module này tới Seeeduino như dưới đây.



| Seeeduino      |  Grove Cable       | Grove - 16 x 2 LCD |
|--------------- |--------------------|-----|
| GND            | Đen              | GND |
| 5V or 3.3V     | Đỏ                | VCC |
| SDA            | Trắng              | SDA |
| SCL            | Vàng             | SCL |


#### Phần mềm

!!!Chú thích
    Nếu đây là lần đầu tiên bạn làm việc với Arduino, chúng tôi chắc chắn khuyên bạn nên xem [Bắt đầu với Arduino](http://wiki.seeedstudio.com/Getting_Started_with_Arduino/) trước khi bắt đầu.


- **Bước 1.** Tải xuống thư viện [Grove-LCD RGB Backlight](https://github.com/Seeed-Studio/Grove_LCD_RGB_Backlight/archive/master.zip) từ Github.


!!!Lời khuyên
         Grove - 16 x 2 LCD chia sẻ cùng một thư viện với [Đèn nền RGB-LCD RGB] (http://wiki.seeedstudio.com/Grove-LCD_RGB_Backlight/). Cách sử dụng của chúng gần như giống nhau, ngoại trừ màn hình LCD Grove - 16 x 2 không hỗ trợ API màu RGB, chẳng hạn như **setRGB()**.


- **Bước 2.** Tham khảo [How to install library](http://wiki.seeedstudio.com/How_to_install_Arduino_Library) để cài đặt thư viện cho Arduino.

- **Bước 3.** Khởi động lại Arduino IDE. Mở ví dụ, bạn có thể mở nó theo ba cách sau:
    1. Mở nó trực tiếp trong Arduino IDE thông qua đường dẫn: **File --> Examples --> Grove - LCD RGB Backlight --> HelloWorld**. 
    ![](https://github.com/SeeedDocument/Grove-16x2_LCD_Series/raw/master/img/path_1.jpg)
    
    2. Mở nó trong máy tính của bạn bằng cách nhấp vào **HelloWorld.ino** mà bạn có thể tìm thấy trong thư mục**XXXX\Arduino\libraries\Grove_LCD_RGB_Backlight-master\examples\HelloWorld**, **XXXX** là vị trí bạn đã cài đặt Arduino IDE.
    ![](https://github.com/SeeedDocument/Grove-16x2_LCD_Series/raw/master/img/path_2.jpg)
    
    3. Hoặc, bạn chỉ cần nhấp vào biểu tượng ![](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/copy.jpg) ở góc trên bên phải của khối mã để sao chép đoạn mã sau vào bản phác thảo mới trong Arduino IDE.


```C++
#include <Wire.h>
#include "rgb_lcd.h"

rgb_lcd lcd;

/*
const int colorR = 255;
const int colorG = 0;
const int colorB = 0;
*/

void setup() 
{
    // set up the LCD's number of columns and rows:
    lcd.begin(16, 2);
    
    //lcd.setRGB(colorR, colorG, colorB);
    
    // Print a message to the LCD.
    lcd.print("hello, world!");

    delay(1000);
}

void loop() 
{
    // set the cursor to column 0, line 1
    // (note: line 1 is the second row, since counting begins with 0):
    lcd.setCursor(0, 1);
    // print the number of seconds since reset:
    lcd.print(millis()/1000);

    delay(100);
}

/*********************************************************************************************************
  END FILE
*********************************************************************************************************/
```

!!!Chú ý
        1** Các tập tin thư viện có thể được cập nhật. Mã này có thể không áp dụng được cho tệp thư viện đã cập nhật, vì vậy chúng tôi khuyên bạn nên sử dụng hai phương pháp đầu tiên.  
        2** Vì loạt **Grove - 16 x 2 LCD** đều là đèn nền đơn sắc, nên bạn cần nhận xét mã liên quan đến màu RGB. Trong mã demo ở trên, tức là, dòng 6 và dòng 17.

- **Bước 4.** Tải lên bản demo. Nếu bạn không biết cách tải lên mã, vui lòng kiểm tra [How to upload code](http://wiki.seeedstudio.com/Upload_Code/).


!!!Kết quả
        Nếu mọi việc suôn sẻ, bạn sẽ thấy màn hình LCD hiển thị câu kinh điển: xin chào thế giới.



## Nguồn

- **[Zip]** [Grove-LCD RGB Backlight Library](https://github.com/Seeed-Studio/Grove_LCD_RGB_Backlight/archive/master.zip)

- **[PDF]** [JDH_1804_Datasheet](https://github.com/SeeedDocument/Grove-16x2_LCD_Series/raw/master/res/JDH_1804_Datasheet.pdf)



## Dự án
Đây là Video giới thiệu về sản phẩm này, các bản demo đơn giản, bạn có thể dùng thử.

<iframe width="560" height="315" src="https://www.youtube.com/embed/3slfeHKSSCw?rel=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>


**Trực quan hóa dữ liệu vận chuyển với Google Map**：Chúng tôi sử dụng mèo Wio LTE.1 để theo dõi GPS vận chuyển và các thông tin khác. Đối với chuỗi lạnh, chúng ta có thể theo dõi vị trí GPS cùng với nhiệt độ và độ ẩm. Đối với xe đạp, chúng ta có thể theo dõi vị trí GPS cùng với tốc độ nghe. 

<iframe frameborder='0' height='327.5' scrolling='no' src='https://project.seeedstudio.com/SeeedStudio/transportation-data-visualization-with-google-map-517ce4/embed' width='350'></iframe>


**Hình dung ô nhiễm khí quyển**：Vấn đề ô nhiễm không khí thu hút ngày càng nhiều sự chú ý. Lần này chúng tôi đã cố gắng theo dõi PM2.5 bằng Wio LTE và Cảm biến Laser PM2.5 mới.

<iframe frameborder='0' height='327.5' scrolling='no' src='https://project.seeedstudio.com/SeeedStudio/atmospheric-pollution-visualization-1940f4/embed' width='350'></iframe>


## Hỗ trợ kỹ thuật

Vui lòng gửi bất kỳ vấn đề kỹ thuật vào [diễn đàn](http://forum.seeedstudio.com/) của chúng tôi.

<br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>