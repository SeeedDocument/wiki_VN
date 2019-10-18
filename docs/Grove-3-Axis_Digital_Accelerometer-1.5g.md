---
name: Grove - 3-Axis Digital Accelerometer(±1.5g)
category: Sensor
bzurl: https://seeedstudio.com/Grove-3-Axis-Digital-Accelerometer(±1.5g)-p-765.html
oldwikiname: Grove_-_3-Axis_Digital_Accelerometer(±1.5g)
prodimagename: 3_aix_acc.jpg
bzprodimageurl: http://statics3.seeedstudio.com/images/101020039 1.jpg
surveyurl: https://www.research.net/r/Grove-3-Axis_Digital_Accelerometer-1_5g
sku: 101020039
tags: grove_i2c, io_3v3, io_5v, plat_duino, plat_linkit, plat_wio
---

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><div class="center">
<div class="floatnone">
<img src="https://raw.githubusercontent.com/SeeedDocument/Grove-3-Axis_Digital_Accelerometer-1.5g/master/img/3_aix_acc.jpg" />
</div>
</div></td>
<td><div class="center">
<div class="floatnone">
<img src="https://raw.githubusercontent.com/SeeedDocument/Grove-3-Axis_Digital_Accelerometer-1.5g/master/img/Grove-3-Axis_v1.3.jpg" />
</div>
</div></td>
</tr>
<tr class="even">
<td><div style=": center">
Grove - 3-Axis Digital Accelerometer v1.2
</div></td>
<td><div style=": center">
Grove - 3-Axis Digital Accelerometer v1.2b
</div></td>
</tr>
</tbody>
</table>

Gia tốc kế kỹ thuật số 3 trục là phần quan trọng trong các dự án như phát hiện định hướng, phát hiện cử chỉ và phát hiện chuyển động. Máy đo gia tốc kỹ thuật số 3 trục (± 1,5g) này dựa trên mô-đun tiêu thụ năng lượng thấp của Freescale, MMA7660FC. Nó có tính năng sống sót sốc cao tới 10.000g và các mẫu có thể định cấu hình trên mỗi giây. Đối với các ứng dụng hào phóng không yêu cầu phạm vi đo quá lớn, đây là một lựa chọn tuyệt vời vì nó bền, tiết kiệm năng lượng và tiết kiệm chi phí.


[![](https://raw.githubusercontent.com/SeeedDocument/common/master/Get_One_Now_Banner.png)](http://www.seeedstudio.com/Grove-3-Axis-Digital-Accelerometer(%C2%B11.5g)-p-765.html)


Các thông số kỹ thuật
--------------

-   Điện áp hoạt động: 3.0 - 5.5V
-   Dòng ở chế độ nghỉ: 0.4μA
-   Dòng ở chế độ chờ: 2μA
-   Dòng ở chế độ hoạt động: 47 μA at 1 ODR
-   Phạm vi kiểm tra: ±1.5g
-   Độ nhạy: 21LSB/g
-   Thư viện tương thích Suli

!!!Mẹo
    Thông tin chi tiết về các module Grove vui lòng tham khảo [Hệ thống Grove](http://wiki.seeedstudio.com/Grove_System/)

Các nền tảng được hỗ trợ
-------------------

| Arduino                                                                                             | Raspberry Pi                                                                                             | BeagleBone                                                                                      | Wio                                                                                               | LinkIt ONE                                                                                         |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/arduino_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/raspberry_pi_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/bbg_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/wio_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/linkit_logo.jpg) |

!!!Chú ý
    Các nền tảng được đề cập ở trên được hỗ trợ như chỉ dẫn của phần mềm của module hoặc khả năng tương thích về mặt lý thuyết. Chúng tôi chỉ cung cấp thư viện phần mềm hoặc các ví dụ cho nền tảng Arduino trong hầu hết các trường hợp. Không thể cung cấp thư viện phần mềm / mã demo cho tất cả các nền tảng MCU. Do đó, người dùng phải viết thư viện phần mềm của riêng họ.



Demo
-------------

### Với [Arduino](/Arduino "Arduino")

Ở đây chúng tôi sẽ chỉ cho bạn cách lấy dữ liệu thô và dữ liệu được đo bằng "g" từ cảm biến này.

Kết nối mô-đun này với cổng I2C của Grove - Base Shield thông qua cáp Grove.

<div class="admonition note">
<p class="admonition-title">Chú ý</p>
Nếu bạn muốn kích hoạt chức năng Ngắt của module này, bạn cần kết nối bảng hàn INT mà chúng tôi đã tạo ra trên bảng với một chân của Arduino có khả năng Ngắt dịch vụ thường xuyên.
</div>

![](https://raw.githubusercontent.com/SeeedDocument/Grove-3-Axis_Digital_Accelerometer-1.5g/master/img/Digital_Accelerometer_Sensor_Connector1.5g.jpg)

Cài đặt thư viện mà chúng tôi cung cấp trong phần [Resources](/Grove-3-Axis_Digital_Accelerometer-1.5g#resources).

Mở mã trực tiếp bằng đường dẫn:File -> Example ->DigitalAccelerometer_MMA7660FC ->MMA7660FC_Demo.

Trong chương trình này, thông tin tăng tốc được gửi từ cảm biến đến Seeeduino qua bus I2C và sau đó Seeeduino in chúng lên màn hình nối tiếp.
Mở màn hình nối tiếp để kiểm tra kết quả.

![](https://raw.githubusercontent.com/SeeedDocument/Grove-3-Axis_Digital_Accelerometer-1.5g/master/img/Grove-3-Axis_Digital_Accelerometer-1.5g-.jpg)

Đầu ra của cảm biến này bao gồm hai phần: dữ liệu thô và thông tin gia tốc 3 trục được chuyển đổi thành đơn vị trọng lực, "g".


### Với Raspberry Pi

1.Bạn nên có một quả mâm xôi pi và một grovepi hoặc grovepi +.

2.Bạn nên hoàn thành cấu hình môi trường phát triển, nếu không hãy làm theo [tại đây](/GrovePi_Plus).

3.Kết nối

-   Cắm cảm biến vào ổ cắm Grovepi i2c-x (1 ~ 3) bằng cách sử dụng cáp Grove.

4.Điều hướng đến thư mục của các bản demo:

       cd yourpath/GrovePi/Software/Python/

-   Để xem mã

```
    nano grove_i2c_accelerometer.py   # "Ctrl+x" to exit #
```
```
    import time
    import grovepi

    # Connect the Grove Accelerometer (+/- 1.5g) to any I2C port eg. I2C-1
    # Can be found at I2C address 0x4c
    # SCL,SDA,VCC,GND

    while True:
        try:
            print grovepi.acc_xyz()
            time.sleep(.5)

        except IOError:
            print "Error"
```

5.Chạy demo.
```
    sudo python grove_i2c_accelerometer.py
```

Tài liệu tham khảo
---------

Dưới đây là hai con số giúp bạn hiểu ý nghĩa vật lý của kết quả.

Hình đầu tiên là về hướng của mỗi trục:
![](https://raw.githubusercontent.com/SeeedDocument/Grove-3-Axis_Digital_Accelerometer-1.5g/master/img/MMA7660_Direction.jpg)

Hình thứ hai cho một số ví dụ

![](https://raw.githubusercontent.com/SeeedDocument/Grove-3-Axis_Digital_Accelerometer-1.5g/master/img/Sensing_Direction_1.jpg)

Nguồn
---------

-   [Datasheet of MMA7660FC](https://raw.githubusercontent.com/SeeedDocument/Grove-3-Axis_Digital_Accelerometer-1.5g/master/res/MMA7660FC.pdf)
-   [Grove - 3-Axis Digital Accelerometer Eagle File](https://raw.githubusercontent.com/SeeedDocument/Grove-3-Axis_Digital_Accelerometer-1.5g/master/res/Grove-3-Axis_Digital_Accelerometer-1.5g-Eagle_File.zip)
-   [github repository for 3-Axis Digital Accelerometer(±1.5g)](https://github.com/Seeed-Studio/Accelerometer_MMA7660)


## Dự án

**Nghiêng quạt kích hoạt quay nhẹ** Thanh màu LED cầm tay phản ứng với chuyển động rung của bạn. Có thêm quạt và báo động.

<iframe frameborder='0' height='327.5' scrolling='no' src='https://www.hackster.io/chuartdo/tilt-activated-spinning-fan-light-stick-e05cec/embed' width='350'></iframe>

**Lean Green RC Sailing Machine**

Một thiết bị được kết nối Internet điều khiển các servo và gửi các cập nhật cảm biến (GPS / con quay / accel / la bàn) trong thời gian thực qua liên kết di động GSM.

<iframe frameborder='0' height='327.5' scrolling='no' src='https://www.hackster.io/anemoi/lean-green-rc-sailing-machine-2cdde5/embed' width='350'></iframe>

<!-- This Markdown file was created from http://www.seeedstudio.com/wiki/Grove_-_3-Axis_Digital_Accelerometer(±1.5g) -->

## Hỗ trợ kỹ thuật
Vui lòng gửi bất kỳ vấn đề kỹ thuật vào [diễn đàn](http://forum.seeedstudio.com/) của chúng tôi. <br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>