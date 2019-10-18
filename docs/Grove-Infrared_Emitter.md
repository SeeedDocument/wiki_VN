---
name: Grove - Infrared Emitter
category: Actuator
bzurl: https://seeedstudio.com/Grove-Infrared-Emitter-p-993.html
oldwikiname: Grove_-_Infrared_Emitter
prodimagename: Grove-Infrared_Emitter.jpg
bzprodimageurl: http://statics3.seeedstudio.com/images/101020026 1.jpg
surveyurl: https://www.research.net/r/Grove-Infrared_Emitter
sku: 101020026
tags: grove_digital, io_3v3, io_5v, plat_duino, plat_pi, plat_wio
---

![](https://github.com/SeeedDocument/Grove-Infrared_Emitter/raw/master/img/main.jpg)

Bộ phát hồng ngoại được sử dụng để truyền tín hiệu hồng ngoại thông qua đèn LED hồng ngoại, trong khi có ** Bộ thu hồng ngoại ** để nhận tín hiệu ở phía bên kia. Một đèn LED hồng ngoại giống như bất kỳ đèn LED nào khác, với màu sắc tập trung vào khoảng 940nm. Chúng tôi không chỉ có thể sử dụng bộ phát để truyền dữ liệu hoặc lệnh mà còn mô phỏng các điều khiển từ xa để điều khiển thiết bị gia đình của bạn bằng Arduino. Bộ phát hồng ngoại có thể truyền tín hiệu đáng tin cậy đến 10 mét. Ngoài 10 mét, máy thu có thể không nhận được tín hiệu. Chúng tôi thường sử dụng hai Groves - [Bộ thu hồng ngoại](http://wiki.seeedstudio.com/Grove-Infrared_Receiver) và Grove - Bộ phát hồng ngoại để làm việc cùng nhau.




<p style=":center"><a href="http://www.seeedstudio.com/Grove-Infrared-Emitter-p-993.html" target="_blank"><img src="https://raw.githubusercontent.com/SeeedDocument/Seeed-WiKi/master/docs/images/get_one_now_small.png" width="210" height="41"  border=0 /></a></p>




## Phiên bản

Phiên bản sản phẩm | Các thay đổi |	Ngày phát hành
--|--|--
Grove - Infrared Emitter v1.0	| Ban đầu |	 01/11/2015
Grove - Infrared Emitter v1.1	| Thay đổi vị trí ống truyền hồng ngoại  |	24/07/2016
Grove - Infrared Emitter v1.2	| Thay đổi giá trị của C1 để làm cho nguồn điện ổn định hơn  |	14/12/2016

## Ứng dụng
- Thiết bị điều khiển từ xa hồng ngoại có yêu cầu công suất cao
- Hệ thống truyền khí miễn phí
- Nguồn hồng ngoại cho máy đếm quang và đầu đọc thẻ

##Các thông số kỹ thuật

| Thông số               | Giá trị   |
|-------------------------|---------------|
| Điện áp hoạt động       | 3.3/5V        |
| Bước sóng đỉnh          | 940nm         |
| Góc của một nửa cường độ | ϕ = ± 17°     |
| Cường độ bức xạ      | 72 mW/sr      |
| Khoảng cách          | 10 meter(MAX) |
| Nhiệt độ hoạt động   | -40℃ to +80℃  |
| Kích thước                    | 20mmX20mm     |

!!!Mẹo
    Thông tin chi tiết về các module Grove vui lòng tham khảo [Hệ thống Grove](http://wiki.seeedstudio.com/Grove_System/)
    



## Các nền tảng được hỗ trợ

| Arduino                                                                                             | Raspberry Pi                                                                                             | BeagleBone                                                                                      | Wio                                                                                               | LinkIt ONE                                                                                         |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/arduino_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/raspberry_pi_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/bbg_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/wio_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/linkit_logo_n.jpg) |

!!!Chú ý
    Các nền tảng được đề cập ở trên được hỗ trợ như chỉ dẫn của phần mềm của module hoặc khả năng tương thích về mặt lý thuyết. Chúng tôi chỉ cung cấp thư viện phần mềm hoặc các ví dụ cho nền tảng Arduino trong hầu hết các trường hợp. Không thể cung cấp thư viện phần mềm / mã demo cho tất cả các nền tảng MCU. Do đó, người dùng phải viết thư viện phần mềm của riêng họ.



## Getting Started

Grove - Bộ phát hồng ngoại có thể gửi dữ liệu trong khi Grove - Bộ thu hồng ngoại sẽ nhận được chúng.

### Đối với Arduino

!!!Chú thích
    Nếu đây là lần đầu tiên bạn làm việc với Arduino, chúng tôi chắc chắn khuyên bạn nên xem [Bắt đầu với Arduino](http://wiki.seeedstudio.com/Getting_Started_with_Arduino/) trước khi bắt đầu.

#### Phần cứng

- **Bước 1.** Chuẩn bị những thứ dưới đây:

| Seeeduino V4.2 | Base Shield| Grove - Infrared Emitter | Grove - Infrared Receiver
|--------------|-------------|-----------------|-----|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/seeeduinoX2.png)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/baseshiledX2.png)|![enter image description here](https://github.com/SeeedDocument/Grove-Infrared_Emitter/raw/master/img/thumbnail.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Infrared_Receiver/raw/master/img/little.jpg)|
|[Get One Now](http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html)|[Get One Now](https://www.seeedstudio.com/Base-Shield-V2-p-1378.html)|[Get One Now](https://www.seeedstudio.com/Grove-Infrared-Emitter-p-993.html)|[Get One Now](https://www.seeedstudio.com/Grove-Infrared-Receiver-p-994.html)|

- **Step 2.** Kết nối Grove - Infrared Emitter tới cổng **D3** của một Grove-Base Shield.
              
- **Step 3.** Kết nối Grove - Infrared Receiver tới cổng **D2** của một Grove-Base Shield khác.

- **Bước 4.** Cắm Grove - Base Shield vào Seeeduino.

- **Bước 5.** Kết nối Seeeduino tới PC qua một cáp USB.


![](https://github.com/SeeedDocument/Grove-Infrared_Emitter/raw/master/img/connect.jpg)


!!!Chú ý
Nếu chúng tôi không có Grove Base Shield, chúng tôi cũng có thể kết nối trực tiếp module này tới Seeeduino như dưới đây.



| Seeeduino       | Grove - Infrared Emitter |
|---------------|-------------------------|
| 5V           | Đỏ                     |
| GND           | Đen                   |
| Không nối | Trắng                   |
| D3            | Vàng                  |


| Seeeduino       | Grove - Infrared Receiver |
|---------------|-------------------------|
| 5V           | Đỏ                     |
| GND           | Đen                   |
| Không nối | Trắng                   |
| D2            | Vàng                  |



#### Phần mềm

- **Bước 1.** Tải xuống  [IRSendRev-master library](https://github.com/Seeed-Studio/IRSendRev)  từ Github.

- **Bước 2.** Tham khảo [How to install library](http://wiki.seeedstudio.com/How_to_install_Arduino_Library) để cài đặt thư viện cho Arduino.

- **Bước 3.** Khởi động lại Arduino IDE. Mở ví dụ `recv` qua đường dẫn: **File->Examples->Grove - Infrared Receiver  And Emitter->recv**. 

![](https://github.com/SeeedDocument/Grove-Infrared_Receiver/raw/master/img/path.png)


Hoặc bạn có thể mở một sketch mới và sao chép mã dưới đây vào Arduino IDE của bạn.

```c++

#include <IRSendRev.h>

#define BIT_LEN         0
#define BIT_START_H     1
#define BIT_START_L     2
#define BIT_DATA_H      3
#define BIT_DATA_L      4
#define BIT_DATA_LEN    5
#define BIT_DATA        6

const int pinRecv = 2;              // ir receiver connect to D2

void setup()
{
    Serial.begin(115200);
    IR.Init(pinRecv);
    Serial.println("init over");
}

unsigned char dta[20];

void loop()
{
    if(IR.IsDta())                  // get IR data
    {
        IR.Recv(dta);               // receive data to dta

        Serial.println("+------------------------------------------------------+");
		Serial.print("LEN = ");
        Serial.println(dta[BIT_LEN]);
        Serial.print("START_H: ");
        Serial.print(dta[BIT_START_H]);
        Serial.print("\tSTART_L: ");
        Serial.println(dta[BIT_START_L]);
        
        Serial.print("DATA_H: ");
        Serial.print(dta[BIT_DATA_H]);
        Serial.print("\tDATA_L: ");
        Serial.println(dta[BIT_DATA_L]);
        
        Serial.print("\r\nDATA_LEN = ");
        Serial.println(dta[BIT_DATA_LEN]);
        
		Serial.print("DATA: ");
        for(int i=0; i<dta[BIT_DATA_LEN]; i++)
        {
            Serial.print("0x");
            Serial.print(dta[i+BIT_DATA], HEX);
            Serial.print("\t");
        }
        Serial.println();
		
		Serial.print("DATA: ");
        for(int i=0; i<dta[BIT_DATA_LEN]; i++)
        {
            Serial.print(dta[i+BIT_DATA], DEC);
            Serial.print("\t");
        }
        Serial.println();
        Serial.println("+------------------------------------------------------+\r\n\r\n");
    }
}

```

- **Step 4.** Tải bản demo `recv` lên seeeduino với Grove - Bộ thu hồng ngoại. Nếu bạn không biết cách tải lên mã, vui lòng kiểm tra [how to upload code](http://wiki.seeedstudio.com/Upload_Code/).

- **Step 5.** Mở ví dụ `send` qua đường dẫn: **File->Examples->Grove - Infrared Receiver  And Emitter->send**. 

Hoặc bạn có thể mở một sketch mới và sao chép mã dưới đây vào Arduino IDE của bạn.


```
#include <IRSendRev.h>

#define BIT_LEN         0
#define BIT_START_H     1
#define BIT_START_L     2
#define BIT_DATA_H      3
#define BIT_DATA_L      4
#define BIT_DATA_LEN    5
#define BIT_DATA        6

const int ir_freq = 38;                 // 38k

unsigned char dtaSend[20];

void dtaInit()
{
    dtaSend[BIT_LEN]        = 11;			// all data that needs to be sent
    dtaSend[BIT_START_H]    = 179;			// the logic high duration of "Start"
    dtaSend[BIT_START_L]    = 90;			// the logic low duration of "Start"
    dtaSend[BIT_DATA_H]     = 11;			// the logic "long" duration in the communication
    dtaSend[BIT_DATA_L]     = 33;			// the logic "short" duration in the communication
    
    dtaSend[BIT_DATA_LEN]   = 6;			// Number of data which will sent. If the number is other, you should increase or reduce dtaSend[BIT_DATA+x].
    
    dtaSend[BIT_DATA+0]     = 128;			// data that will sent
    dtaSend[BIT_DATA+1]     = 127;
    dtaSend[BIT_DATA+2]     = 192;
    dtaSend[BIT_DATA+3]     = 63;
	dtaSend[BIT_DATA+4]     = 192;
    dtaSend[BIT_DATA+5]     = 63;
}

void setup()
{
    dtaInit();
}

void loop()
{
    IR.Send(dtaSend, 38);
    
    delay(2000);
}


```

- **Bước 6.** Tải lên bản demo `send` cho seeeduino với Grove - Infrared Emitter. 


- **Step 7.** Mở **Serial Monitor** của Arduino IDE bằng cách nhấp vào **Tool-> Serial Monitor**. Hoặc nhấn phím ++ ctrl + shift + m ++ cùng một lúc.


Nếu mọi việc suôn sẻ. Kết quả sẽ như sau:

![](https://github.com/SeeedDocument/Grove-Infrared_Emitter/raw/master/img/results.png)



## Nguồn

- **[Zip]**  [Grove-Infrared Emitter eagle files](https://raw.githubusercontent.com/SeeedDocument/Grove-Infrared_Emitter/master/res/Grove-Infrared_Emitter_eagle_files.zip)
- **[Lib]**  [IR Send and Receiver Library](https://github.com/Seeed-Studio/IRSendRev)
- **[Pdf]**  [TSAL6200 Datasheet](http://www.vishay.com/docs/81010/tsal6200.pdf)

## Dự án

**LaunchPad đến giao tiếp LaunchPad**: Gửi văn bản từ một LaunchPad đến một người khác bằng cách sử dụng bộ phát và nhận Grove IR!

<iframe frameborder='0' height='327.5' scrolling='no' src='https://www.hackster.io/ctroberts/ir-launchpad-to-launchpad-communication-0dd109/embed' width='350'></iframe>




## Hỗ trợ kỹ thuật
Vui lòng gửi bất kỳ vấn đề kỹ thuật vào [diễn đàn](http://forum.seeedstudio.com/) của chúng tôi. <br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>