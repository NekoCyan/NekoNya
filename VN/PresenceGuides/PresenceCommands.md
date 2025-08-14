# Discord Tool - Black Market Tool (Business Market Tool)

_Lệnh Hiện Diện_

<hr>

#### Định nghĩa cú pháp:

-   `{}` - Trường bắt buộc.
-   `[]` - Trường tùy chọn | Bạn có thể để trống trong lệnh.
-   `URL` - Bất kỳ Link Web/URL nào.
-   `IMAGE_URL` - Link/URL hình ảnh (Bạn cũng có thể tải hình ảnh lên Discord và lấy URL hình ảnh từ đó).
-   `NỘI_DUNG` - Bất kỳ văn bản nào.
-   `LOẠI` - Loại hiện diện | Như name, details, state, v.v... xem trong [Loại Hiện Diện](presence_example.png) hoặc hình ảnh bên dưới.

#### Loại hiện diện

<img id="presence-example" src="presence_example.png" alt="Loại hiện diện" width="600" />

#### Ví dụ lệnh với định nghĩa cú pháp:

> nếu lệnh là `!!command {NỘI_DUNG}` và bạn muốn `NỘI_DUNG` là `Hello`, thì bạn sẽ nhập `!!command Hello`.
> nếu lệnh là `!!set {URL} [NỘI_DUNG]` và bạn muốn `NỘI_DUNG` là rỗng, thì bạn sẽ nhập `!!set https://www.youtube.com/watch?v=dQw4w9WgXcQ`.

<hr>

## Lệnh

_Nhấp vào từng phần bên dưới để mở rộng và xem chi tiết._

<details>
    <summary><strong>Hiển thị cài đặt | Hiển thị cài đặt hiện diện của bạn.</strong></summary>
    
```diff
!!hiendien hienthi
```
</details>

<details>
    <summary><strong>Đặt một loại | Thay đổi loại cụ thể trong cài đặt hiện diện.</strong></summary>

Vui lòng chuyển đến [Thiết lập loại hiện diện](#thiết-lập-loại-hiện-diện) bên dưới để xem thêm chi tiết lệnh.

</details>

<details>
    <summary><strong>Xóa một loại | Xóa loại cụ thể trong cài đặt hiện diện.</strong></summary>
    
```diff
!!hiendien xoa {LOẠI}
```
</details>

<details>
    <summary><strong>Hiển thị hiện diện | Bật hiển thị hiện diện của bạn trong hồ sơ.</strong></summary>
    
```diff
!!hiendien bat
```
</details>

<details>
    <summary><strong>Dừng hiển thị hiện diện | Dừng hiển thị hiện diện của bạn trong hồ sơ.</strong></summary>
    
```diff
!!hiendien tat
```
</details>

<details>
    <summary><strong>Đặt lại cài đặt | Xóa tất cả loại trong cài đặt hiện diện (để trống tất cả).</strong></summary>
    
```diff
!!hiendien caidatlai
```
</details>

## Thiết lập loại hiện diện.

Phần này là về việc thiết lập các loại hiện diện của bạn bằng cách sử dụng lệnh, xem [Định nghĩa cú pháp](#định-nghĩa-cú-pháp) để xem lệnh nhập và [NHẤP VÀO ĐÂY](#loại-hiện-diện) để xem loại mà bạn muốn thiết lập.

<details>
    <summary><strong>Loại: Name.</strong></summary>
    
```diff
!!hiendien chinhsua name {NỘI_DUNG}
```
</details>

<details>
    <summary><strong>Loại: Details.</strong></summary>
    
```diff
!!hiendien chinhsua details {NỘI_DUNG}
```
</details>

<details>
    <summary><strong>Loại: State.</strong></summary>
    
```diff
!!hiendien chinhsua state {NỘI_DUNG}
```
</details>

<details>
    <summary><strong>Loại: Large (Cũng với văn bản lớn).</strong></summary>
    
```diff
!!hiendien chinhsua large {IMAGE_URL} [NỘI_DUNG]
```
`NỘI_DUNG` trong lệnh này được phép để trống.
</details>

<details>
    <summary><strong>Loại: Small (Cũng với văn bản nhỏ).</strong></summary>
    
```diff
!!hiendien chinhsua small {IMAGE_URL} [NỘI_DUNG]
```
`NỘI_DUNG` trong lệnh này được phép để trống.
</details>

<details>
    <summary><strong>Loại: Button1.</strong></summary>
    
```diff
!!hiendien chinhsua button1 {URL} {NỘI_DUNG}
```
</details>

<details>
    <summary><strong>Loại: Button2.</strong></summary>
    
```diff
!!hiendien chinhsua button2 {URL} {NỘI_DUNG}
```
</details>

<details>
    <summary><strong>Loại: Time.</strong></summary>
    
```diff
!!hiendien chinhsua time {THỜI_GIAN}
```
Trong trường `THỜI_GIAN`, bạn được phép đặt một trong những điều sau:
- `1` - Hiển thị thời gian hoạt động kể từ khi khởi động hệ thống.
- `TIMEZONE` - Hiển thị thời gian hiện tại trong múi giờ cụ thể.
  
Bạn có thể chọn múi giờ của mình trong liên kết [https://en.wikipedia.org/wiki/List_of_tz_database_time_zones](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones) và đặt văn bản theo `TZ identifier` trên trang web vào trường `THỜI_GIAN`.
<br>
Ví dụ: nếu múi giờ của tôi với UTC offset là +07:00, tôi sẽ đặt `Asia/Ho_Chi_Minh` vào trường `THỜI_GIAN`, vì vậy nó sẽ là:
<br>
`!!hiendien chinhsua time Asia/Ho_Chi_Minh`
</details>

## Lưu ý: Nếu Hiện Diện của bạn đang bật nhưng bạn đã thực hiện thay đổi trong cài đặt, Hiện Diện của bạn sẽ tự động bị tắt, và sau khi hoàn tất Cài đặt của bạn, vui lòng bật lại.
