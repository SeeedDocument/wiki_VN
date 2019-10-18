---
name: Grove - Infrared Receiver
category: Sensor
bzurl: https://seeedstudio.com/Grove-Infrared-Receiver-p-994.html
oldwikiname: Grove_-_Infrared_Receiver
prodimagename: Grove-Infrared_Receiver.jpg
bzprodimageurl: http://statics3.seeedstudio.com/images/101020016 1.jpg
surveyurl: https://www.research.net/r/Grove-Infrared_Receiver
sku: 101020016
tags: grove_digital, io_3v3, io_5v, plat_duino
---



![](https://github.com/SeeedDocument/Grove-Infrared_Receiver/raw/master/img/Grove-Infrared_Receiver.jpg)

Bộ thu hồng ngoại được sử dụng để nhận tín hiệu hồng ngoại và cũng được sử dụng để phát hiện điều khiển từ xa. Có một máy dò hồng ngoại trên Bộ thu hồng ngoại được sử dụng để lấy ánh sáng hồng ngoại phát ra từ Bộ phát hồng ngoại. Máy dò hồng ngoại có bộ giải mã bên trong tìm kiếm IR được điều chế ở 38 KHz. Bộ thu hồng ngoại có thể nhận tín hiệu tốt trong vòng 10 mét. Nếu hơn 10 mét, máy thu có thể không nhận được tín hiệu. Chúng tôi thường sử dụng hai Groves - Bộ thu hồng ngoại và [Grove - Bộ phát hồng ngoại] (http://wiki.seeedstudio.com/Grove-Infrared_Emitter) để hoạt động cùng nhau.

[![](https://raw.githubusercontent.com/SeeedDocument/common/master/Get_One_Now_Banner.png)](http://www.seeedstudio.com/Grove-Infrared-Receiver-p-994.html)



## Phiên bản

Phiên bản sản phẩm | Thay đổi |	Ngày phát hành
--|--|--
Grove - Infrared Receiver v1.0	| Ban đầu |	01/11/2015
Grove - Infrared Receiver v1.1	| Thay đổi màn hình  |24/07/2016



##Các thông số kỹ thuật

-   Điện áp: 3.3-5V
-   Khoang cách:10m

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

- **Bước 2.** Kết nối Grove - Infrared Emitter tới cổng **D3** của một Grove-Base Shield.
              
- **Bước 3.** Kết nối Grove - Infrared Receiver tới cổng **D2** của một Grove-Base Shield khác.

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

- **Bước 1.** Tải xuống [IRSendRev-master library](https://github.com/Seeed-Studio/IRSendRev)  từ Github.

- **Bước 2.** Tham khảo [How to install library](http://wiki.seeedstudio.com/How_to_install_Arduino_Library) để cài đặt thư viện cho Arduino

- **Bước 3.**  Khởi động lại Arduino IDE. Mở ví dụ `recv` qua đường dẫn: **File->Examples->Grove - Infrared Receiver  And Emitter->recv**. 

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

- **Bước 4.** Tải bản demo `recv` lên seeeduino với Grove - Bộ thu hồng ngoại. Nếu bạn không biết cách tải lên mã, vui lòng kiểm tra [how to upload code](http://wiki.seeedstudio.com/Upload_Code/).

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


- **Bước 7.** Mở **Serial Monitor** của Arduino IDE bằng cách nhấp vào **Tool-> Serial Monitor**.Hoặc nhấn phím ++ ctrl + shift + m ++ cùng một lúc.


Nếu mọi việc suôn sẻ. Kết quả sẽ như sau:


![](https://github.com/SeeedDocument/Grove-Infrared_Emitter/raw/master/img/results.png)



## Nguồn


- **[Zip]**  [Grove - Infrared Receiver eagle files](https://raw.githubusercontent.com/SeeedDocument/Grove-Infrared_Receiver/master/res/Grove-Infrared_Receiver_eagle_files.zip)
- **[Lib]**  [IR Send and Receiver Library](https://github.com/Seeed-Studio/IRSendRev)
- **[Lib]**  [IR Receive Library for LinkIt ONE](https://github.com/Seeed-Studio/IR_Recv_LinkIt_ONE)
- **[Pdf]**  [TSOP282 Datasheet](http://www.vishay.com/docs/82491/tsop382.pdf)


## Dự án

**IR LaunchPad đến giao tiếp LaunchPad**:Gửi văn bản từ một LaunchPad đến một người khác bằng cách sử dụng bộ phát và nhận Grove IR!
<iframe frameborder='0' height='327.5' scrolling='no' src='https://www.hackster.io/ctroberts/ir-launchpad-to-launchpad-communication-0dd109/embed' width='350'></iframe>


## Hỗ trợ kỹ thuật
Vui lòng gửi bất kỳ vấn đề kỹ thuật vào [diễn đàn](http://forum.seeedstudio.com/) của chúng tôi. <br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>