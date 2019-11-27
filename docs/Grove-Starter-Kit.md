# Grove - Starter Kit v3  
Grove là một nền tảng mô-đun điện tử để có thể tạo các mẫu một cách tiện lợi và nhanh chóng. Nhiều cấu hình không cần đến hàn hay bảng mạch tạm thời vẫn có thể lắp ráp. Ta chỉ cần kết nối đơn giản các mô-đun Grove với Grove Shield và tận dụng các mẫu code đã cung cấp cho từng mô-đun là được. Grove Starter Kit bao gồm một loạt các cảm biến và bộ khởi động, hỗ trợ âm thanh, ánh sáng, chuyển động, cảm nhận và nhiều chế độ tương tác khác. Vì vậy, bạn có thể bắt đầu nhiều dự án cùng lúc.  





## Về Grove  
Grove là một bộ công cụ đã được kiểm duyệt và có thể sử dụng luôn. Giống như Lego,  nó sử dụng phương pháp xếp chồng các khối để liên kết các linh kiện điện tử. So với phương pháp truyền thống, khi mà học cách sử dụng một bảng mạch tạm thời và các linh kiện điện tử khác nhau để lắp ráp một dự án khá phức tạp, Grove đơn giản hóa và cô đọng lại quá trình học tập đáng kể. Hệ thống Grove bao gồm một Base Sheild cùng kết nối chuẩn hóa với các mô-đun khác nhau.

Base Sheild cho phép những kết nối đơn giản từ bất kỳ vi xử lý đầu ra hoặc đầu vào nào từ các mô-đun Grove. Mỗi một mô-đun Grove chỉ có một chức năng duy nhất, ví dụ như một nút đơn giản hoặc một cảm biến nhịp tim phức tạp hơn. Mỗi mô-đun sẽ đi kèm với tài liệu rõ ràng và code demo để giúp bạn bắt đầu một cách nhanh chóng.  





## Tìm hiểu về Arduino  
Nếu đây là lần đầu bạn sử dụng Arduino, bạn cần hoàn thành các bước sau:  

- [Bắt đầu với Arduino : Getting Started with Arduino](http://wiki.seeedstudio.com/Getting_Started_with_Arduino)
- [Cài đặt vi xử lý của bạn : Install your microcontroller](http://wiki.seeedstudio.com/Getting_Started_with_Seeeduino)
- [Tải về và đưa vào Grove – Starter Kit Sketchbook : Download and import the Grove - Starter Kit Sketchbook](http://wiki.seeedstudio.com/How_To_Use_Sketchbook)  

Địa chỉ tải về của Grove - Starter Kit Sketchbook [ở đây](https://github.com/Seeed-Studio/Sketchbook_Starter_Kit_V2.0) .  
Bây giờ thì bạn đã sẵn sàng để khám phá hệ sinh thái Grove.  





## Danh sách các phần  
- 1*Base Shield
- 1*Grove - LCD RGB Backlight
- 1*Grove - Smart Relay
- 1*Grove - Buzzer
- 1*Grove - Sound Sensor
- 1*Grove - Touch Sensor
- 1*Grove - Rotary Angle Sensor
- 1*Grove - Temperature Sensor
- 1*Grove - LED
- 1*Grove - Light Sensor
- 1*Grove – Button
- 1*DIP LED Blue-Blue
- 1*DIP LED Green-Green
- 1*DIP LED Red-Red
- 1*Mini Servo
- 10*Grove Cables
- 1*9V to Barrel Jack Adapter
- 1*Grove starter kit Manual
- 1*Green Plastic Box  





## Chi tiết các mô-đun  



### Grove - Base Shield
Chúng ta hãy bắt đầu với Grove Base Sheild. "Grove-Base Shield" là phiên bản mới của "Electronic Brick Shield". Base Shield này tương thích với Seeeduino v 3.0 (168p và 328p), cũng như với Arduino UNO và Duemilanove. Có 16 cổng Grove trên một Base Sheild, được chia thành bốn chức năng: Analog (tương tự) (4), Digital (số) (7), I2C (4), và UART (1).  

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Starter_Kit_v3/master/wiki_VN/base_shield.jpg)

- **Cổng Digital**  
Như hình ảnh cho thấy, có bảy cổng Digital có nhãn là D2-D8. Mỗi một cổng này xử lý một cặp chân digital (2/3... 8/9) trên Uno Arduino. Chúng có thể được sử dụng để đọc cảm biến digital (ví dụ: nút Push) hoặc điều khiển bộ truyền động Digital (hoặc Analog, qua PWM). Trong mọi trường hợp, mỗi cổng chỉ có thể xử lý hai trạng thái logic: 0 hoặc 1.  

- **Cổng Analog**  
Ở phía bên tay trái là bốn cổng Grove để đọc Analog. Cảm biến Analog có thể trả về từ 0 đến 1023. So với các cảm biến Digital chỉ trả về 0 hoặc 1, các kết quả từ Analog chi tiết hơn và chính xác hơn.  

- **Cổng I2C**  
I2C là giao thức bus tốc độ thấp, có thể truyền dữ liệu qua hai dây: SCL và SDA. SCL là đường truyền xung clock để đồng bộ hóa truyền dữ liệu qua bus I2C, còn SDA là đường truyền dữ liệu. Sơ đồ sau minh họa khung của bus I2C. Để biết thông tin chi tiết về cách sử dụng Grove-Base Shield của bạn, hãy đến link [Base Shield V2](http://wiki.seeedstudio.com/Base_Shield_V2) .  



### Grove - LCD RGB Backlight ( Đèn nền LCD RGB)  

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Starter_Kit_v3/master/wiki_VN/LCD1.jpg)

Đèn nền Grove - LCD RGB hỗ trợ hiển thị văn bản và sử dụng các ký tự do người dùng xác định. Nó cho phép bạn đặt màu đèn nền với giao diện Grove đơn giản và súc tích. Nó sử dụng phương thức I2C để giao tiếp với Arduino của bạn. Vì vậy, số lượng chân cần thiết để trao đổi dữ liệu và điều khiển đèn nền co lại từ ~ 10 xuống còn 2, để lại nhiều khả năng I / O hơn cho các nhiệm vụ khó khăn khác.  

**Ví dụ**  
Ví dụ dưới đây chỉ ra cho bạn cách in văn bản lên màn hình và đổi màu sắc của đèn nền. Tìm theo đường dẫn dưới đây:  
*File -> Sketchbook -> Grove_RGB_Backlight_LCD -> HelloWorld*  

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Starter_Kit_v3/master/wiki_VN/LCD2.jpg)

**Tips**  
Đây là một màn hình LCD 16x2. Nó có khả năng hiển thị hai hàng văn bản mười sáu ký tự, hỗ trợ các ngôn ngữ bao gồm tiếng Anh và tiếng Nhật. Bạn cũng có thể tùy chỉnh và xây dựng các ký tự đặc biệt bằng cách xác định các mẫu hiển thị của chúng. Bạn có thể tìm thấy một ví dụ về việc tạo một ký tự tùy chỉnh ở đây:  
https://github.com/Seeed-Studio/Grove_LCD_RGB_Backlight/archive/master.zip  



### Grove – Rơle  

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Starter_Kit_v3/master/wiki_VN/relay1.jpg)

Rơle là một công cụ hữu ích để giúp cho khả năng điều khiển của Arduino của bạn lớn hơn! Đưa tín hiệu điều khiển qua giao diện Grove và Rơle sẽ mở hoặc đóng mạch ngoài được kết nối với các đầu nối vít. Điện áp của mạch ngoài có thể chạy lên đến 220V! Vì vậy, hãy sử dụng rơle và bắt đầu một số dự án thực sự khó khăn!  

**Ví dụ**  
Ví dụ chỉ ra cách bạn có thể điều khiển một rơle thông qua một nút : *File -> Sketchbook -> Grove_Relay*  

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Starter_Kit_v3/master/wiki_VN/relay2.jpg)

**Tips**  
Rơle là một công tắc cơ được điều khiển bằng điện tử. Kích thước của rơle thay đổi tùy theo khả năng dẫn điện của nó. Rơle càng lớn (về cơ bản chỉ là phần hộp nhựa) thì khả năng dẫn điện của nó càng lớn.  

<font color=red>Vui lòng thực hiện cẩn thận khi làm việc với điện áp lưới điện - nếu gặp khó khăn, hãy liên hệ với chuyên gia như thợ điện chuyên nghiệp để được giúp đỡ.</font>  

Để biết thêm thông tin chi tiết về cách sử dụng Grove - Rơle, bạn có thể đến link sau [Grove – Relay page](http://wiki.seeedstudio.com/Grove-Relay) .  



### Grove – Buzzer (Còi Buzzer)  

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Starter_Kit_v3/master/wiki_VN/buzzer1.jpg)  

Buzzer là một Grove đơn giản nhưng sử dụng rất thú vị. Nó là loa áp điện kết hợp cùng với một mạch điều khiển đơn giản. Nếu nó được kết nối với đầu ra digital, nó sẽ phát ra âm báo khi đầu ra cao. Ngoài ra, nó có thể được kết nối với đầu ra analog (thực tế, là digital được hiệu chỉnh độ rộng xung) để tạo ra các âm và hiệu ứng khác nhau.  

**Ví dụ**  
Bạn có thể sử dụng mã cho nút Grove để tạo tiếng bíp từ còi khi bạn nhấn nút. Tuy nhiên, còi Buzzer Grove có thể thú vị hơn nhiều, nó còn có thể phát các bài hát! Đây là một ví vụ được cung cấp bởi Oomlout.com, còi Buzzer sẽ phát ra một bài hát thiếu nhi - “Twinkle Twinkle, Little Star”. Ví dụ ở đường dẫn dưới đây :  
*File > Sketchbook > Grove_Buzzer*  

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Starter_Kit_v3/master/wiki_VN/buzzer2.jpg)  

**Tips**  
Làm thế nào để còi buzzer Piezo hoạt động? Thông thường, trong mỗi một loa Piezo buzzer thì đều có hai tấm gốm. Khi truyền điện áp vào, các tấm gốm sẽ hút hoặc đẩy nhau, từ đó khiến chúng rung lên. Sự chuyển động của các tấm này gây ra sự rung động của không khí (tức là âm thanh).  Khi tần số rung thay đổi , tần số âm thanh cũng thay đổi.  
Để biết thêm thông tin về cách sử dụng Grove – Buzzer của bạn, bạn có thể đến link sau [Grove - Buzzer page](http://wiki.seeedstudio.com/Grove-Buzzer) .  



### Grove - Sound Sensor ( Cảm biến âm thanh)  
Mô đun Cảm biến âm thanh là một micrô đơn giản. Dựa vào bộ khuếch đại LM58 và micrô điện tử, nó có thể được sử dụng để phát hiện mức độ âm thanh trong môi trường.  

**Ví dụ**  
Mã code cho cảm biến âm thanh Grove có thể được sử dụng để điều khiển đèn LED có độ sáng phản ánh cường độ âm thanh xung quanh.  
*File -> Sketchbook -> Grove_Sound_Sensor*  

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Starter_Kit_v3/master/wiki_VN/sound.jpg)  

**Tips**  
Micro điện thu thập các cường độ âm thanh ở mọi tần số, và lúc này chiết áp sẽ đóng vai trò là người gác cửa. Chẳng hạn, khi bạn xoay nó theo chiều kim đồng hồ đến cực điểm, nó sẽ cho phép tất cả mọi thứ đi qua. Còn khi bạn quay nó hoàn toàn ngược chiều kim đồng hồ, thì không có gì có thể đi qua cả.  
Để biết thêm thông tin về cách sử dụng Grove – Sound Sensor của bạn, bạn có thể đến link sau [Grove - Sound Sensor page](http://wiki.seeedstudio.com/Grove-Sound_Sensor) .  



### Grove - Touch Sensor (Cảm biến cảm ứng)  

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Starter_Kit_v3/master/wiki_VN/touch1.jpg)  

Grove - Touch Sensor (Cảm biến cảm ứng) cho phép bạn thay thế việc ấn nút bằng sự tiếp xúc trên bề mặt. Khi một ngón tay ở gần, nó có thể phát hiện sự thay đổi của điện dung. Vì vậy, cho dù ngón tay của bạn chạm trực tiếp hay chỉ ở gần nó, Bộ cảm biến Grove - Touch sẽ có đầu ra là HIGH.  

**Ví dụ**  
Mã của Grove- Button được hoạt động theo mô đun này.  
Tìm ví dụ theo đường dẫn sau: *File -> Sketchbook -> Grove_Buzzer*  

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Starter_Kit_v3/master/wiki_VN/touch2.jpg)  

**Tips**  
Đây là một sự thay thế cho nút tạm thời. Cảm biến cảm ứng Grove phát hiện sự thay đổi điện dung trong vùng hình tròn; ngón tay bạn càng gần khu vực đó, sự thay đổi điện dung càng lớn. Ngay cả khi có một tờ giấy giữa ngón tay bạn và cảm biến, nó vẫn có thể hoạt động đáng tin cậy.  
Để biết thêm thông tin về cách sử dụng Grove – Touch Sensor của bạn, bạn có thể đến link sau [Grove - Touch Sensor page](http://wiki.seeedstudio.com/Grove-Touch_Sensor) .  



### Grove - Rotary Angle Sensor ( Cảm biến góc quay )  

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Starter_Kit_v3/master/wiki_VN/angle1.jpg)  

Chiết áp Grove tạo ra đầu ra tương tự giữa 0 và VCC (3,3 hoặc 5 VDC). Góc quay có sự thay đổi tuyến tính về giá trị trong phạm vi bán kính là 300 độ. Giá trị điện trở là 10k ohms, phù hợp cho việc sử dụng Arduino. Nó cũng có thể hiểu như là một “cảm biến góc quay”.  

**Ví dụ**  
Ví dụ này có thể mô tả cho bạn cách đọc được giá trị của một cảm biến góc quay : *File > Sketchbook > Grove_Rotary_Angle_Sensor*  

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Starter_Kit_v3/master/wiki_VN/angle2.jpg)  

**Tips**  
Một chiết áp xoay trông rất giống với một bộ mã hóa quay, nhưng chúng không giống nhau. Một chiết áp xoay thực chất là một chiết áp trượt, được chế tạo như hình tròn. Trong loại analog, nó phản hồi phần của điện trở được sử dụng bằng tiếp điểm trượt.  
Để biết thêm thông tin về cách sử dụng Grove – Rotary Angle Sensor của bạn, bạn có thể đến link sau [Grove - Rotary Angle Sensor page](http://wiki.seeedstudio.com/Grove-Rotary_Angle_Sensor) .  



### Grove – Temperature Sensor ( Cảm biến nhiệt độ)  

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Starter_Kit_v3/master/wiki_VN/temp1.jpg)  

Cảm biến nhiệt độ Grove sử dụng một điện trở nhiệt để trả về nhiệt độ của môi trường. Sau đó, board của chúng ta sẽ chuyển đổi giá trị điện áp đo bằng chân đầu vào analog này thành nhiệt độ. Phạm vi hoạt động được là -40 đến 125 độ C.  

**Ví dụ**  
Mã trong ví dụ sau đây hiển thị cách chuyển đổi đầu ra thô của cảm biến sang giá trị nhiệt độ. Bạn có thể nhìn thấy dữ liệu đầu ra dưới dạng độ C trong màn hình nối tiếp : *File > Sketchbook > Grove_Temperature_Sensor*  

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Starter_Kit_v3/master/wiki_VN/temp2.jpg)  

**Tips**  
Cảm biến nhiệt độ Grove được dùng để phát hiện nhiệt độ môi trường.  
Để biết thêm thông tin về cách sử dụng Grove - Temperature Sensor của bạn, bạn có thể đến link [Grove - Temperature Sensor](http://wiki.seeedstudio.com/Grove-Temperature_Sensor) .  



### Grove – LED (Đèn Led)  

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Starter_Kit_v3/master/wiki_VN/LED1.jpg)  

Grove - LED được thiết kế cho người mới bắt đầu Arduino / Seeeduino để giám sát các điều khiển từ các cổng digital. Nó có thể được gắn vào bề mặt hộp hoặc bàn của bạn một cách dễ dàng và được sử dụng làm đèn báo hiệu cho nguồn điện hoặc tín hiệu.  

**Ví dụ**  
Trong ví dụ này chúng tôi thực hiện một đèn LED với hiệu ứng hô hấp:  
*File -> Sketchbook -> Grove_LED*

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Starter_Kit_v3/master/wiki_VN/LED2.jpg)  

**Tips**  
Chúng tôi chuẩn bị ba màu của bóng đèn LED cho bạn, bạn có thể có được màu sắc bạn muốn bằng cách thay đổi đèn LED trên ổ cắm nhỏ Grove - LED. Đèn LED có cực âm ở mặt phẳng của bóng đèn và cực dương ở cạnh tròn của bóng đèn. Cực dương cần được cài đặt tương ứng với dấu "+" để đèn LED hoạt động chính xác.  
Để biết thêm thông tin về cách sử dụng Grove - LED của bạn, bạn có thể đến link  [Grove - Red LED](http://wiki.seeedstudio.com/Grove-Red_LED) .  



### Grove - Light Sensor (Cảm biến ánh sáng)  

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Starter_Kit_v3/master/wiki_VN/light1.jpg)  

Cảm biến ánh sáng, còn được gọi là điện trở quang (LDR). Thông thường, điện trở của cảm biến ánh sáng sẽ giảm khi cường độ ánh sáng xung quanh tăng lên.  

**Ví dụ**  
Ví dụ này sẽ bật đèn LED khi cường độ ánh sáng giảm xuống dưới ngưỡng đã được cài đặt trước:  
*File -> Sketchbook -> Grove_Light_Sensor*  

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Starter_Kit_v3/master/wiki_VN/light2.jpg)  

**Tips**  
Đầu ra của cảm biến ánh sáng tương tự nằm trong khoảng từ 0 đến 1023, nhưng nó không tuyến tính đối với cường độ ánh sáng xung quanh.  
Để biết thêm thông tin về cách sử dụng Grove - Light Sensor của bạn, bạn có thể đến link [Grove - Light Sensor](http://wiki.seeedstudio.com/Grove-Light_Sensor) .



### Grove – Button ( Nút )  

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Starter_Kit_v3/master/wiki_VN/button1.jpg)  

Phiên bản mới của mô-đun nút này chứa bao gồm một nút độc lập, có cấu hình là điện trở pull-down, luôn sẵn sàng để sử dụng với bộ vi điều khiển như đầu vào digital. Nút báo hiệu dây SIG và NC thì không được sử dụng trong mô-đun Grove này.  

**Ví dụ**  
Ví dụ này đưa ra cho bạn cách bật hoặc tắt một đèn LED dựa vào một nút.  
*File -> Sketchbook -> Grove_Button*

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Starter_Kit_v3/master/wiki_VN/button2.jpg)  

**Tips**  
“Tạm thời” có nghĩa là bật lại sau khi nhấn. Nút sẽ trả về HIGH khi nhấn và LOW khi thả ra.  



### Grove - Servo  

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Starter_Kit_v3/master/wiki_VN/servo1.jpg)  

Đây là một bộ khởi động mà có thể điều khiển chính xác được vị trí .  

**Ví dụ**  
Chúng tôi đã chuẩn bị một ví dụ về cách mà chúng tôi sử dụng một chiết áp để điều khiển vị trí của servo:  
*File --> Sktechbook --> Servo*

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Starter_Kit_v3/master/wiki_VN/servo2.jpg)  

**Tips**  
Grove - Servo có một số tùy chọn gắn kết với phần cứng cho các mục đích khác nhau: bạn có thể sử dụng chúng để điều khiển một chiếc quạt nhỏ, nâng cấp một đối tượng, hoặc bắt chước một chiếc đồng hồ.  






## Dự án demo  




### 1. A Cup Of Flowers - Một chiếc cốc hoa  

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Starter_Kit_v3/master/wiki_VN/a_cup_of_flowers/1.jpg)  

**Miêu tả**  
Bạn có muốn một cốc hoa để làm dịu trái tim mệt mỏi của mình? Dự án này được tạo thành từ Grove - LED và Grove -  Touch Sensor( Cảm biến cảm ứng) . Khi chạm vào cảm biến, những đèn LED đáng yêu đó sẽ chiếu ánh sáng với hiệu ứng ấm áp và thoải mái đến bạn.  

**Danh sách vật liệu**  
1. Arduino x 1;
2. Grove – Base Shield x 1;
3. Grove – LED x 6;
4. Grove – Touch Sensor x 1;
5. 6 x 6cm Color paper x 6;
6. 9V battery & 9V battery clip x 1.  

**Ghi chú**  
Số lượng đèn LED là tùy ý. Trong bộ kit cơ bản có ba chiếc. Tuy nhiên, bạn có thể tăng hoặc giảm số lượng tùy thuộc vào thể tích cốc của bạn. Tôi có một chiếc cốc lớn ở đây, vì vậy tôi đã thêm ba cái đèn LED nữa từ trang web của chúng tôi.  

**Các bước**  

1. **Gấp bông hoa**  
![](https://raw.githubusercontent.com/SeeedDocument/Grove_Starter_Kit_v3/master/wiki_VN/a_cup_of_flowers/2.jpg)

   Chọn một mẫu hoa bạn thích và làm theo các bước của nó để tạo ra một số mẫu. Sử dụng Google Search có thể sẽ giúp đỡ rất nhiều trong việc tìm kiếm. Có rất nhiều người muốn chia sẻ sản phẩm thủ công của họ trên Internet như những người yêu thích origami hay các nghệ sĩ thủ công.  
   Ở đây tôi chọn hoa tulip, nhưng hoa hướng dương, hoa hồng hay hoa ly cũng rất thú vị!  
   Khi gấp nụ, bạn cần chừa một lỗ nhỏ trên nút để dây cáp Grove có thể đi qua.

2. **Chuẩn bị**  
![](https://raw.githubusercontent.com/SeeedDocument/Grove_Starter_Kit_v3/master/wiki_VN/a_cup_of_flowers/3.jpg)

   Kết nối các nụ và cảm biến cảm ứng bằng dây cáp Grove 10cm vào Grove - Base Shield. Sau đó, tải mã code lên bộ điều khiển của bạn.  

3. **Truyền năng lượng và ổn định**  
![](https://raw.githubusercontent.com/SeeedDocument/Grove_Starter_Kit_v3/master/wiki_VN/a_cup_of_flowers/4.jpg)

   Sử dụng pin 9V để cung cấp năng lượng cho những bông hoa và đặt chúng vào trong chiếc cốc. Đã xong! Hãy cùng thưởng thức chiếc cốc hoa của bạn!  



### 2. How You Doing!  

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Starter_Kit_v3/master/wiki_VN/how_you_doing/1.jpg)  

**Miêu tả**  
Bạn sẽ chào người bạn của mình như thế nào ?Big Chief sẽ nói rằng  “Còn điều gì tuyệt vời hơn một chút đung đưa?” Khi một con đồ chơi giấy Big Chief dựa lưng vào con khác, chúng sẽ lắc lư để nói xin chào !  

**Danh sách vật liệu**  
1. Arduini x 1;
2. Grove – Base Shield x 1;
3. Grove – Magnetic Switch x 1;
4. Grove – Vibrator x 1;
5. Paper toys x 2;
6. Magnet x 1;
7. 9V battery & 9V battery clip x 1.

**Chú ý:** Số lượng đèn LED là tùy ý. Trong bộ kit cơ bản có ba chiếc. Tuy nhiên, bạn có thể tăng hoặc giảm số lượng tùy thuộc vào thể tích cốc của bạn. Tôi có một chiếc cốc lớn ở đây, vì vậy tôi đã thêm ba cái đèn LED nữa từ trang web của chúng tôi.  

**Các bước làm**  

1. **In ra**  
![](https://raw.githubusercontent.com/SeeedDocument/Grove_Starter_Kit_v3/master/wiki_VN/how_you_doing/2.jpg)

   Chọn mẫu mà bạn thích trên Internet. Đảm bảo rằng bạn có đủ chỗ cho nam châm hoặc công tắc từ cộng với máy rung. Giống như bông hoa origami ở trên, bạn có thể tìm rất nhiều trên Internet.  

2. **Thêm các bộ phận**  
Thật tập trung khi bạn cắt đồ chơi giấy, chỉ có như vậy thì bạn mới có được một sản phẩm đẹp. Sau đó sẽ là thời gian để thêm các bộ phận cho chúng. Tôi đã dán một cục nam châm ở mặt sau của Big Chief A (Hãy gọi cho nó cái tên này) bằng băng dính hai mặt.  
![](https://raw.githubusercontent.com/SeeedDocument/Grove_Starter_Kit_v3/master/wiki_VN/how_you_doing/3.jpg)
Và đối với Big Chief B, tôi đã dán một công tắc từ trên lưng  - cùng vị trí với Big Chief A và một cái máy rung trên chân của nó.  
![](https://raw.githubusercontent.com/SeeedDocument/Grove_Starter_Kit_v3/master/wiki_VN/how_you_doing/4.jpg)  

3. **Dán chúng vào với nhau**  
![](https://raw.githubusercontent.com/SeeedDocument/Grove_Starter_Kit_v3/master/wiki_VN/how_you_doing/5.jpg)

   Làm theo tờ giấy hướng dẫn đã in một cách cẩn thận. Cắm các dây cáp Grove vào các mô đun sử dụng cho Big Chef B. Sau đó bạn sẽ có hai chiếc đồ chơi giấy dễ thương như trên.  

4. **Tải chương trình lên**  
![](https://raw.githubusercontent.com/SeeedDocument/Grove_Starter_Kit_v3/master/wiki_VN/how_you_doing/6.jpg)

   Tải mã code dưới đây vào Arduino. Bằng cách này, bạn sẽ mang lại sự sống cho chúng.  


**Chuẩn hóa** -  Hình dạng ghép hình có thể mở rộng, các đầu nối 4 chân thống nhất, lưới lỗ vít, miếng hàn cạnh có thể giảm phát triển trùng lặp và tái sử dụng trong các dự án khác nhau để giảm tác động môi trường.    

**Nhỏ gọn** – kích thước từ 2cm * 2 cm, sự kết hợp không có mối hàn, các bộ phần được lắp trên bề mặt và khoảng cách cáp là 2.0mm.  

**Thân thiện** – kết nối dễ dàng, dễ dàng sử dụng và tiếp cận, có các chế độ mở rộng khác nhau và các DIY, thư viện và mã demo đều mở.  

**Phong phú** - Rất nhiều lựa chọn các mạch phổ biến từ cảm biến cơ bản (nút, LED) đến chuyên nghiệp (Gyro, La bàn), luôn tiếp tục bổ sung theo yêu cầu, có sự đóng góp của bên thứ 3 và có thể tái sử dụng.  

**Dựa trên cộng đồng** – đáp ứng nhu cầu thông qua bỏ phiếu, dân chủ hóa các thiết kế, chia sẻ các dự án và công thức, kinh doanh theo mô hình chia sẻ lợi nhuận, có cho thuê và tái sử dụng.






## Câu hỏi thường gặp  

**Q1: Nó có hoạt động với bo mạch Intel Galileo Gen 1 không?**  
A1: Có, bạn có thể sử dụng bộ công cụ này trên bo mạch Intel Galileo Gen1 / Gen2 hay Edison cho Arduino.
 
**Q2: Tuy màu sắc phía sau hoạt động tốt, nhưng không có gì hiển thì trên đèn nền Grove - RGB LCD cả.**  
A2:Vui lòng kiểm tra xem công tắc nguồn (3.3V / 5V) có ở phía 5V hay không.
Tham khảo thêm

[Sch pdf](https://github.com/SeeedDocument/Grove_Starter_Kit_v3/raw/master/res/Grove-Starter_Kit_v3_sch_pdf.zip)  
[Sch Eagle]()  
[Grove - Button Source File](https://github.com/SeeedDocument/Grove_Starter_Kit_v3/raw/master/res/Grove-Button_v1.0_Source_File.zip)  
[Grove - LED Source File](https://github.com/SeeedDocument/Grove_Starter_Kit_v3/raw/master/res/Grove-LED_v1.0_Source_File.zip)  
[Grove - Buzzer Source File](https://github.com/SeeedDocument/Grove_Starter_Kit_v3/raw/master/res/Grove-Buzzer_v1.0_Source_File.zip)  
[Grove - Rotary Angle Sensor Source File](https://github.com/SeeedDocument/Grove_Starter_Kit_v3/raw/master/res/Grove-Rotary_Angle_Sensor_v1.2.zip)  
[Grove - Relay Source File](https://github.com/SeeedDocument/Grove_Starter_Kit_v3/raw/master/res/Grove-Relay_v1.2_Eagle.zip)  
[Base Shield Source File](https://github.com/SeeedDocument/Grove_Starter_Kit_v3/raw/master/res/Base_Shield_v2.zip)  
[Grove - Sound Sensor Source File](https://github.com/SeeedDocument/Grove_Starter_Kit_v3/raw/master/res/Grove-Sound_Sensor_v1.3_eagle.zip)  
[Grove - Buzzer Source File](https://github.com/SeeedDocument/Grove_Starter_Kit_v3/raw/master/res/Grove-Buzzer_V1.1_eagle.zip)  

Lời cảm ơn  
Chúng tôi muốn bày tỏ lòng biết ơn tới Rich Morin, người đã sửa đổi tài liệu này bằng ngữ pháp và từ ngữ phù hợp hơn.  
Hỗ trợ về kỹ thuật  
Vui long gửi bất kỳ vấn đề về kỹ thuật nào xảy ra đến [forum](http://forum.seeedstudio.com/) của chúng tôi.