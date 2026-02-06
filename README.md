# Mạch kết nối MKE-M15 Bluetooth UART Module

## Giới thiệu sản phẩm
MKE-M15 Bluetooth UART Module là mạch kết nối không dây sử dụng giao tiếp UART, cho phép bổ sung khả năng kết nối Bluetooth cho các mạch điều khiển một cách nhanh chóng và tiện lợi. Thông qua module này, hệ thống có thể giao tiếp không dây với máy tính, điện thoại thông minh và các thiết bị hỗ trợ Bluetooth 2.0 và Bluetooth 4.0 (BLE).

Ở chế độ Bluetooth 2.0, Mạch kết nối MKE-M15 Bluetooth UART Module có độ tương thích cao và có thể sử dụng như một giải pháp thay thế cho các module phổ biến HC-05 / HC-06 mà không cần chỉnh sửa chương trình điều khiển. Với Bluetooth 4.0 (BLE), module cho phép kết nối ổn định với hầu hết các smartphone hiện nay chạy Android và iOS như iPhone, iPad…, mở rộng khả năng điều khiển không dây cho các ứng dụng hiện đại.

Mạch kết nối MKE-M15 Bluetooth UART Module sử dụng chuẩn giao tiếp UART quen thuộc và hỗ trợ tập lệnh AT Commands, giúp người dùng dễ dàng cấu hình, kết nối và tích hợp vào hệ thống. Sản phẩm phù hợp cho các ứng dụng điều khiển từ xa, giám sát, truyền dữ liệu không dây, mô hình robot, dự án STEM và đồ án học tập.

Mạch kết nối MKE-M15 Bluetooth UART Module hỗ trợ điện áp điều khiển 3.3V và 5VDC, cho phép kết nối trực tiếp và an toàn với các bo mạch điều khiển phổ biến như Arduino, Raspberry Pi, Jetson Nano, Micro:bit và nhiều nền tảng khác. Sản phẩm đi kèm cáp kết nối 4P XH2.54 – Dupont, đảm bảo kết nối chắc chắn, ổn định và thuận tiện trong quá trình lắp đặt và sử dụng.

## Thông số kỹ thuật
- Điện áp hoạt động: 5VDC
- Điện áp giao tiếp: TTL 3.3VDC/5VDC
- Chuẩn giao tiếp: Digital UART
- Baudrate Default: 9600, N, 8, 1
- Hỗ trợ cấu hình qua bộ tập lệnh AT Commands.
- Chuẩn kết nối Bluetooth: Bluetooth 2.0 và Bluetooth 4.0 (BLE)
- Khoảng cách truyền nhận tối đa: 30m
- Tương thích hệ điều hành: Windows / Android / IOS
- Khả năng tương thích:
  - Arduino
  - Raspberry Pi
  - Jetson Nano
  - Micro:bit
  - Và các board điều khiển 3.3/5VDC khác
- Thiết kế mạch:
  - Ổn định, chống nhiễu
  - Phù hợp cho ứng dụng học tập và thực tế
- Đi kèm cáp kết nối: 4P XH2.54–Dupont

## Bộ tập lệnh AT Commands
Nếu muốn thay đổi các thiết lập mặc định (thường không cần thiết), bạn có thể sử dụng bộ tập lệnh cấu hình AT Commands để cấu hình lại cho Mạch thu phát MKE-M15 Bluetooth 3.0 SPP / BLE 4.2 Dual Mode module, tuy nhiên việc này cần sử dụng thêm mạch chuyển USB-UART hoặc lập trình qua Arduino, xin lưu ý thiết lập đúng **Baudrate Default: 9600, N, 8, 1** và sau các lệnh **AT** cần thêm **\r\n**:

## Các chân tín hiệu
<table><thead>
  <tr>
    <th>MKE-M15</th>
    <th>Ghi chú</th>
  </tr></thead>
<tbody>
  <tr>
    <td>GND</td>
    <td>Chân cấp nguồn âm 0VDC</td>
  </tr>
  <tr>
    <td>5V</td>
    <td>Chân cấp nguồn dương 5VDC</td>
  </tr>
  <tr>
    <td>TX</td>
    <td>Chân truyền tín hiệu UART Transmitter</td>
  </tr>
  <tr>
    <td>RX</td>
    <td>Chân nhận tín hiệu UART Receiver</td>
  </tr>
</tbody>
</table>

## Hướng dẫn sử dụng
### Hướng dẫn kết nối
- Cấp nguồn 5VDC cho mạch qua hai chân GND và 5V.
- Kết nối chân RX của Module với chân TX xủa mạch điều khiển.
- Kết nối chân TX của Module với chân RX của mạch điều khiển.

### Hướng dẫn sử dụng với Arduino Uno / Vietduino Uno / ESP32
- Trong **Tools / Library Manager**, tìm và cài đặt bộ thư viện tổng hợp **"MKE_ONE" by MakerEdu.vn**
- Mở chương trình mẫu **"MKE_M15_Bluetooth_Serial_XXX"** tại **File / Examples / MAKEREDU / Module / MKE_M15_Bluetooth**
- Cấu hình board mạch tương ứng là **Arduino Uno / ESP32**, chọn đúng cổng **COM Port** của mạch và nhấn **Upload** để nạp chương trình.
- Cấp nguồn 5VDC cho mạch, kết nối chân TX và RX của Module với chân điều khiển được khai báo trong chương trình.
- Xem kết quả mạch hoạt động theo chương trình đã nạp.

### Hướng dẫn lập trình với Micro:bit (kéo thả khối)

- Khởi động [Microsoft MakeCode](https://makecode.microbit.org/) và **Import** chương trình theo đường link sau: `https://github.com/makereduvn/mke_m15_bluetooth_microbit/`
- Kết nối mạch Micro:bit và **Download** chương trình.
- Cấp nguồn 5VDC cho mạch, kết nối chân TX và RX của Module với chân điều khiển được khai báo trong chương trình.
- Xem kết quả mạch hoạt động theo chương trình đã nạp.

Nếu bắt đầu tự án mới cần cài đặt Extension **MKE_ONE_MICROBIT** trên [Microsoft MakeCode](https://makecode.microbit.org/) theo [hướng dẫn tại đây](https://github.com/makereduvn/MKE_ONE_MICROBIT). Sau khi cài đặt thành công, các khối lệnh của Extension **MKE_ONE_MICROBIT** sẽ xuất hiện trong danh sách block và sẵn sàng để sử dụng.

## Kích thước sản phẩm
![MKE-M15 Bluetooth](/extras/MKE-M15_1.jpg)

## Hình ảnh sản phẩm
![MKE-M15 Bluetooth](/extras/MKE-M15_2.png)
![MKE-M15 Bluetooth](/extras/MKE-M15_3.png)
