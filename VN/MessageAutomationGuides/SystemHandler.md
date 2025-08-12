# Discord Tool - Black Market Tool (Business Market Tool)

_Hướng Dẫn Kiến Thức - System Handler_

<hr>

> Chúng tôi đã giới hạn việc tạo thư mục tối đa là 25 thư mục, vì vậy bạn phải tổ chức các thư mục của mình trên các kênh một cách hợp lý theo hướng dẫn dưới đây.

<hr>

## Có 3 cách để điều khiển việc tạo thư mục

-   Thứ nhất (Được khuyến khích nhất): Tạo tên thư mục theo loại nhóm (như `selling` hoặc `buying`...).

-   Thứ hai (Được khuyến khích): Tạo tên thư mục theo thời gian (như `5m` hoặc `10m`...).

-   Thứ ba (Không tốt): Tạo tên thư mục kết hợp cả loại nhóm và thời gian (như `selling5m` hoặc `buying10m`...).

<i>Tùy thuộc vào tên thư mục, bạn có thể thêm các kênh liên quan đến thư mục đó và xử lý dễ dàng bằng cùng một nội dung tin nhắn cần được gửi.</i>

<br>

## Xử lý thời gian của thư mục (Trong trường hợp thời gian hoạt động sai trên thư mục)

Đôi khi có một vài bug nhỏ khiến thời gian không hoạt động đúng cách, vì vậy nếu bạn có nhiều kênh trong một thư mục, bạn phải tuân theo quy tắc dưới đây để xử lý thư mục tốt hơn.

```csharp
nếu có hơn 30 kênh, đặt thời gian thành 5m.
nếu có hơn 40 kênh, đặt thời gian thành 7.5m.
nếu có hơn 50 kênh, đặt thời gian thành 10m.
```

> _Mỗi 10 kênh sẽ tăng thời gian thêm 2.5 phút._

## Bộ điều khiển chế độ chậm

Bạn không cần quan tâm về việc chế độ chậm của kênh (trên kênh tin nhắn của Discord) quá ngắn hoặc quá dài cho một thư mục, chúng tôi đã tự động hóa điều này cho bạn như sau.

```csharp
nếu thời gian thư mục = 5m, trong khi chế độ chậm kênh = 30m, hệ thống sẽ chọn 30m thay thế.
nếu thời gian thư mục = 1h, trong khi chế độ chậm kênh = 30m, hệ thống sẽ chọn 1h thay thế.
```

> _Hệ thống sẽ luôn chọn giá trị cao nhất giữa thời gian của thư mục và chế độ chậm của kênh._
