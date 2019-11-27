---
title: Grove Inventor Kit for micro:bit
category: Tutorial
bzurl:  https://www.seeedstudio.com/Grove-Inventor-Kit-for-micro%3Abit-p-2891.html
oldwikiname: Grove_Inventor_Kit_for_micro:bit
prodimagename: https://statics3.seeedstudio.com/seeed/file/2017-06/bazaar492598_8.jpg
surveyurl: https://www.research.net/r/Grove_Inventor_Kit_for_microbit
sku:    110060762
---
![](https://github.com/SeeedDocument/Grove_kit_for_microbit/raw/master/img/zoro_im_kitbox.jpg)

BBC micro:bit là một máy tính bỏ túi có thể dễ dàng nhận ra sự sáng tạo của bạn mà không cần có kiến thức về điện và lập trình. Có rất nhiều khả năng sáng tạo mà bạn có thể khai thác bằng micro: bit, từ robot đến nhạc cụ. Tuy nhiên, nếu bạn muốn tạo ra nhiều thứ hơn, chỉ cần 1 micro: bit là không đủ, đó là lý do tại sao chúng tôi giới thiệu Grove Inventor Kit cho micro: bit cho bạn.

Grove Inventor Kit cho Micro:bit mang đến khả năng vô tận cho micro: bit của bạn. Mạch lõi trong bộ công cụ này là tấm chắn Grove cho micro:bit, trong đó bạn có thể sử dụng nhiều module Grove bao gồm cảm biến, màn hìnhm bộ truyền động để tương tác với micro:bit. Nếu bạn chưa bao giờ sử dụng và không biết Grove là gì, thì đây là phần giới thiệu Grove. Tất cả những gì bạn cần biết là với Grove, không cần hàn hay dây nhảy nữa. Tạo mẫu của bạn sẽ dễ dàng và thuận tiện hơn nhiều.

Chúng tôi đã chuẩn bị 8 module Grove để giúp bạn bắt đầu với micro: bit. Với các module grove này, bạn có thể đo khoảng cách và hiển thị nó, sử dụng cử chỉ để phát nhạc khác nhau hoặc tạo một người bảo vệ thông minh cho bàn hoặc phòng của bạn. Chúng tôi đã chuẩn bị tất cả các thư viện (gói) cần thiết để tải xuống miễn phí. Nếu bạn là người mới bắt đầu sử dụng micro: bit, đừng lo lắng vì chúng tôi cũng đã chuẩn bị 12 dự án khác nhau có thể dạy bạn từng bước. Nếu bạn là người dùng nâng cao, bộ tài liệu này sẽ giúp bạn dự án sáng tạo hơn những người khác.


!!!Chú ý
    - Điện áp đầu ra của micro: bit là khoảng 3.0V, sử dụng pin microbit hoặc pin AA để cấp nguồn cho mạch có thể gây ra sự cố cho các module Grove đòi hỏi điện áp đầu vào cao và dòng điện (ví dụ Grove - Ranger siêu âm). Để làm cho các loại Grove này hoạt động tốt, vui lòng sử dụng cổng micro-USB trên tấm chắn Grove cho microbit để cấp nguồn cho mạch.





[![](https://github.com/SeeedDocument/Seeed-WiKi/raw/master/docs/images/300px-Get_One_Now_Banner-ragular.png)](https://www.seeedstudio.com/Grove-Inventor-Kit-for-micro%3Abit-p-2891.html)

##  Đặc trưng

  - Vỏ bọc mở rộng với các thiết bị ngoại vi phong phú;
  - 10 module Grove được chọn để làm việc với micro:bit;
  - 12 dự án tuyệt vời giúp bạn bắt đầu nhanh chóng;
  - Tài liệu hướng dẫn tốt.

##  Tổng quan phần cứng


![](https://github.com/SeeedDocument/Grove_kit_for_microbit/raw/master/img/first_im.jpg)

###  **Danh sách các bộ phận**
| Tên các bộ phận | Số lượng |
|--------------------------|-----|
|Grove Shield for micro:bit|  1  |
|Grove - Rotary Angle Sensor(P)| 1 |
|Grove - Speaker | 1 |
|Grove - Ultrasonic Ranger| 1 |
|Grove - Light Sensor v1.2| 1 |
|Grove - WS2812 Waterproof LED Strip - 30 LEDs 1 meter| 1 |
|Grove - Gesture | 1 |
|Grove - 4-Digit Display| 1 |
|Grove - Red LED| 1 |
|Micro USB Cable - 48cm| 1 |
|12 Projects Manual| 1 |
|Alligator Cable| 10 |
|Grove Cable| 7 |


##  Bắt đầu

###  Nguyên tắc cơ bản với Micro:bit

Bạn cần biết một số kiến thức cần thiết nếu đây là lần đầu tiên bạn tham gia với Micro: bit. Bạn có thể click [ **tại đây** ](https://microbit.org/code/) để nhận thông tin về Micro:bit.

Micro:bit cung cấp hai loại trình soạn thảo - JavaScript Block Editor và Python Editor. JavaScript Block Editor hỗ trợ lập trình đồ họa, thật dễ học. Vì vậy, Hướng dẫn này dựa trên JavaScript Block Editor.

Đây là hai bước đơn giản trước khi bạn bắt đầu với bộ sản phẩm của chúng tôi, sau đó chúng ta có thể bắt đầu chương trình.

####  Bước 1. Mở Editor

Vui lòng click để mở **[JavaScript Block Editor](https://makecode.microbit.org/)** , và bạn sẽ thấy một trang web lập trình đồ họa.


####  Bước2.Thêm Grove Package
  - Click vào bánh răng ở góc trên bên phải > chọn **Add Package**

  ![](https://github.com/SeeedDocument/Grove_kit_for_microbit/raw/master/img/0-1.png)

  - Nhập dự án URL: **github.com/seeed-studio/pxt-grove**

  ![](https://github.com/SeeedDocument/Grove_kit_for_microbit/raw/master/img/0-2.png)

  - Bây giờ bạn có thể tìm thấy **Grove**   trên toolbar.

  ![](https://github.com/SeeedDocument/Grove_kit_for_microbit/raw/master/img/0-3.png)

### Demo 1. Nhận diện cử chỉ 

Cảm biến cử chỉ có thể nhận ra 9 cử chỉ khác nhau, trong bản demo này, bạn sẽ học cách hiển thị tên cử chỉ được nhận dạng trên micro: bit.


#### Danh sách các phần

|Tên các phần|số lượng|
|---|---|
|Grove - Gesture|1|
|Grove Shield for micro:bit|1|
|micro:bit|1|
|Grove Universal 4 pin cable|1|
|Micro-USB cable|1|

#### Kết nối

  - Cắm **micro:bit** vào **Grove Shield for micro:bit**.
  - Kết nối Grove-Gesture tới cổng **I2C** của micro:bit thông qua cáp Grove Universal 4 chân.
  - Kết nối micro:bit tới PC qua một cáp Micro-USB.

!!!Cảnh báo

      -Xin vui lòng đảm bảo rằng Mảng LED được úp lên khi bạn cắm micro: bit, hoặc bạn có thể làm hỏng bảng..


![](https://github.com/SeeedDocument/Grove_kit_for_microbit/raw/master/img/Gesture%20Recognition.png)


#### Phần mềm
  - Bước 1:

  Thêm Gesture Block

  ![](https://github.com/SeeedDocument/Grove_kit_for_microbit/raw/master/img/1-1.png)

  - Bước 2:

  Chọn Right, để cảm biến có thể nhận ra khi bạn di chuyển tay từ phải sang trái.

  ![](https://github.com/SeeedDocument/Grove_kit_for_microbit/raw/master/img/1-2.png)

  - Bước 3:

  Thêm khối Basic **show string** và nhúng nó vào khối Gesture. Sau đó nhấp đúp vào "Hello!", thay đổi nó thành "Right".

  ![](https://github.com/SeeedDocument/Grove_kit_for_microbit/raw/master/img/1-3.png)

  - Bước 4:

  Thêm "Left" và "Clockwise" tương tự trên, và nhúng **show icon** vào "Clockwise".

  ![](https://github.com/SeeedDocument/Grove_kit_for_microbit/raw/master/img/1-4.png)

  - Bước 5:

  Khi hoàn thành các bước trên, đổi tên dự án "gesture". Sau đó có thể tải xuống mạch của bạn. Click **Download** trong Bottom left corner, tải xuống file **microbit-gesture.hex** vào flash của MICROBIT.


  ![](https://github.com/SeeedDocument/Grove_kit_for_microbit/raw/master/img/1-5.png)

  Bây giờ bạn có thể chạy demo.

!!!Mẹo
    - Bạn có thể tìm thấy các khối theo màu sắc. Ví dụ, Nếu bạn không có **show icon**,vì nó có màu xanh và Module **Basic** cũng màu xanh, bạn có thể tìm thấy nó ở đó? Đơn giản và hiệu quả phải không?


### Demo 2. Máy đo siêu âm

Trong bản demo này, bạn sẽ học cách sử dụng cảm biến siêu âm để đo khoảng cách và hiển thị giá trị trên màn hình.

#### Danh mục các phần
|Tên từng phần|Số lượng|
|---|---|
|Grove - Ultrasonic Ranger|1|
|Grove - 4-Digit Display|1|
|Grove Shield for micro:bit|1|
|micro:bit|1|
|Grove Universal 4 pin cable|2|
|Micro-USB cable|1|

#### Kết nối

  - Cắm **micro:bit** vào **Grove Shield for micro:bit**.

!!!Cảnh báo
Vui lòng đảm bảo rằng Mảng LED được úp lên khi bạn cắm micro: bit, hoặc bạn có thể làm hỏng bảng.

  - Kết nối Grove-Ultrasonic Ranger tới cổng **P0/P14** của micro:bit qua cáp Grove Universal 4 chân.
  - Kết nối Mần hình Grove-4-Digit tới cổng **P1/P15** của micro:bit qua cáp 4 chân Grove Universal.
  - Kết nối micro:bit tới PC qua cáp Micro-USB.

  ![](https://github.com/SeeedDocument/Grove_kit_for_microbit/raw/master/img/Ultrasonic_Meter.png)

#### Phần mềm

  - Bước 1:

  Thêm khối cơ bản **on start**, sau đó thêm các khối biến **set item to 0**, đổi tên ‘items’ thành ‘Display’. Nếu bạn thêm thành công Grove package, thay thế “0” với khối Grove hiển thị 4 chữ số ở P1 and P15.

  ![](https://github.com/SeeedDocument/Grove_kit_for_microbit/raw/master/img/2-1.png)

  ![](https://github.com/SeeedDocument/Grove_kit_for_microbit/raw/master/img/2-2.png)

  - Bước 2:

  Thêm khối cơ bản mãi mãi, sau đó thêm vật phẩm khối Grove hiển thị số 0, đổi tên ‘item’ thành ‘Display’, đổi ‘0’ với khối Grove Ultrasonic Sensor (tính bằng cm) tại P0.

  - Bước 3:

  Thêm khối dừng cơ bản (ms) (100).

  ![](https://github.com/SeeedDocument/Grove_kit_for_microbit/raw/master/img/2-3.png)

  - Bước 4:

  Đổi tên dự án "Ultrasonic Meter", tải xuống và chạy.


## Nguồn

  [**Grove Inventor Kit for micro:bit User Manual**](https://github.com/SeeedDocument/Grove_kit_for_microbit/blob/master/res/Guide-Grove%20kit%20for%20microbit.pdf)

  [**micro:bit Getting Started Videos**](http://microbit.org/start/)

  [**About micro:bit**](http://microbit.org/about/)

  [**micro:bit Hardware**](http://microbit.org/guide/hardware/)

  [**micro:bit Apps**](http://microbit.org/code/)

  [**Grove Shield for microbit_eagle file.zip**](https://github.com/SeeedDocument/Bazzar_Attachment/raw/master/103030195/202001587_Grove%20Shield%20for%20BBC%20microbit%20V1.2_eagle%20file.zip)
