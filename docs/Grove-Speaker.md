---
name: Grove - Speaker
category: Actuator
bzurl: https://seeedstudio.com/Grove-Speaker-p-1445.html
oldwikiname: Grove_-_Speaker
prodimagename: Grove_Speaker_01.jpg
bzprodimageurl: http://statics3.seeedstudio.com/images/product/Grove Speaker.jpg
surveyurl: https://www.research.net/r/Grove-Speaker
sku: 107020001
tags: grove_digital, io_5v, plat_duino, plat_wio
---

![](https://raw.githubusercontent.com/SeeedDocument/Grove-Speaker/master/img/Grove_Speaker_01.jpg)

Grove- Speaker là một module bao gồm khuếch đại công suất và đầu ra bằng giọng nói. Độ to có thể được điều chỉnh bằng chiết áp trên mạch. Với tần số đầu vào khác nhau, loa lớn tạo ra các âm khác nhau. Mã hóa âm nhạc vào arduino, DIY hộp nhạc của riêng bạn!

[![](https://raw.githubusercontent.com/SeeedDocument/common/master/Get_One_Now_Banner.png)](http://www.seeedstudio.com/Grove-Speaker-p-1445.html)

Đặc tính
-------

-   Điều chỉnh âm lượng
-   Giao diện Grove

!!!Mẹo
    Thông tin chi tiết về các module Grove vui lòng tham khảo [Hệ thống Grove](http://wiki.seeedstudio.com/Grove_System/)


Các thông số kỹ thuật
-------------

| Item            | Min | Điển hình | Max | Đơn vị |
|-----------------|-----|---------|-----|------|
| Điện áp hoạt động | 4.0 | 5.0     | 5.5 | VDC  |
| Điện áp Gain    | -   | -       | 46  | db   |
| Độ rộng băng      | -   | -       | 20  | KHz  |

Các nền tảng được hỗ trợ
-------------------

| Arduino                                                                                             | Raspberry Pi                                                                                             | BeagleBone                                                                                      | Wio                                                                                               | LinkIt ONE                                                                                         |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/arduino_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/raspberry_pi_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/bbg_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/wio_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/linkit_logo_n.jpg) |

!!!Chú ý
    Các nền tảng được đề cập ở trên được hỗ trợ như chỉ dẫn của phần mềm của module hoặc khả năng tương thích về mặt lý thuyết. Chúng tôi chỉ cung cấp thư viện phần mềm hoặc các ví dụ cho nền tảng Arduino trong hầu hết các trường hợp. Không thể cung cấp thư viện phần mềm / mã demo cho tất cả các nền tảng MCU. Do đó, người dùng phải viết thư viện phần mềm của riêng họ.


Sử dụng
-----

### Với Arduino

Loa có thể phát ra nhiều âm thanh như tiếng còi xe, chuông cửa và đánh lửa. Các âm thanh khác nhau dựa trên tần số của tín hiệu đầu vào.

Bạn có thể cung cấp tín hiệu tần số khác nhau cho mô-đun này với Arduino. Arduino tạo ra các tín hiệu này thông qua PWM hoặc thậm chí là ghi và trễ kỹ thuật số. Chúng tôi sẽ chỉ cho bạn cách tạo các tín hiệu này bằng cách sử dụng * delay () *, loa âm trầm 1 ~ 7.

![](https://raw.githubusercontent.com/SeeedDocument/Grove-Speaker/master/img/Tone.jpg)

```
/*macro definition of Speaker pin*/
#define SPEAKER 3

int BassTab[]={1911,1702,1516,1431,1275,1136,1012};//bass 1~7

void setup()
{
    pinInit();
}
void loop()
{
        /*sound bass 1~7*/
    for(int note_index=0;note_index<7;note_index++)
    {
        sound(note_index);
        delay(500);
    }
}
void pinInit()
{
    pinMode(SPEAKER,OUTPUT);
    digitalWrite(SPEAKER,LOW);
}
void sound(uint8_t note_index)
{
    for(int i=0;i<100;i++)
    {
        digitalWrite(SPEAKER,HIGH);
        delayMicroseconds(BassTab[note_index]);
        digitalWrite(SPEAKER,LOW);
        delayMicroseconds(BassTab[note_index]);
    }
}
```
<div class="admonition note">
<p class="admonition-title">Chú ý</p>
Do ảnh hưởng của điện dung, module chỉ có thể phát tín hiệu âm trầm và âm cao không thể phát ra.
</div>

### Với Codecraft

#### Phần cứng

**Bước 1.** Kết nối Grove - Speaker tới cổng D3 trên Base Shield

**Bước 2.** Cắm Base Shield tới Seeeduino/Arduino.

**Bước 3.** Kết nối Seeeduino/Arduino tới PC qua USB.

#### Phần mềm

**Bước 1.** Mở [Codecraft](https://ide.chmakered.com/), thêm hỗ trợ Arduino và kéo một lệnh chính vào vùng làm việc.

!!!Chú ý
   Nếu đây là lần đầu tiên bạn sử dụng Codecraft, hãy xem thêm [Hướng dẫn sử dụng Codecraft bằng Arduino](http://wiki.seeedstudio.com/Guide_for_Codecraft_using_Arduino/).

**Bước 2.** Kéo các khối như hình dưới đây hoặc mở tệp cdc có thể được tải xuống ở cuối trang này.

![](https://github.com/SeeedDocument/Grove-Speaker/raw/master/img/Speaker.png)

Tải chương trình lên Arduino / Seeeduino của bạn.


!!!Kết quả
   Khi mã được tải lên, bạn sẽ nghe thấy loa phát ra âm thanh từ ĐÔ đến SI.

Nguồn
--------

-   [Grove - Speaker Eagle File](https://raw.githubusercontent.com/SeeedDocument/Grove-Speaker/master/res/Grove-Speaker_Eagle_File.zip)
-   [How to generate different tone with MCU](https://raw.githubusercontent.com/SeeedDocument/Grove-Speaker/master/res/Tone.pdf)
-   [Grove\_-\_Speaker\_v1.0\_brd.pdf](https://raw.githubusercontent.com/SeeedDocument/Grove-Speaker/master/res/Grove-Speaker_v1.0_brd.pdf)
-   [Grove\_-\_Speaker\_v1.0\_sch.pdf](https://raw.githubusercontent.com/SeeedDocument/Grove-Speaker/master/res/Grove-Speaker_v1.0_sch.pdf)
-   [LM386 Low Voltage Audio Power Amplifier Datasheet](https://raw.githubusercontent.com/SeeedDocument/Grove-Speaker/master/res/LM386_Low_Voltage_Audio_Power_Amplifier_Datasheet.pdf)
-   [CodeCraft Code](https://github.com/SeeedDocument/Grove-Speaker/raw/master/res/Speaker.zip)


<!-- This Markdown file was created from http://www.seeedstudio.com/wiki/Grove_-_Speaker -->

## Hỗ trợ kỹ thuật
Vui lòng gửi bất kỳ vấn đề kỹ thuật vào [diễn đàn](http://forum.seeedstudio.com/) của chúng tôi. <br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>