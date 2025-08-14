# Discord Tool - Black Market Tool (Business Market Tool)

_Lệnh Người Dùng - Lệnh Cơ Bản_

<hr>

<details open>
    <summary><strong>1. Thêm một Thư mục | Dùng để xử lý thời gian, kênh v.v...</strong></summary>
    
```diff
!!thumuc them TÊN_THƯ_MỤC
```
</details>

<br>

<details open>
    <summary><strong>2. Đặt thời gian | Tiếp tục lặp lại sau khi tin nhắn được gửi mãi mãi ~</strong></summary>
    
```diff
!!thoigian chinhsua THỜI_GIAN
```
Thời gian phải có định dạng `1s`, `2m`, `3h`, `4d` (tức là 1 giây, 2 phút, 3 giờ, 4 ngày).
<br>
Ví dụ: `!!thoigian chinhsua 5m` # Đặt thời gian của thư mục thành 5 phút
</details>

<br>

<details open>
    <summary><strong>3. Thêm một Kênh | Nơi để gửi tin nhắn đến.</strong></summary>
    
```diff
!!kenh them ID_CHANNEL
```
*Bạn có thể thêm nhiều kênh cùng lúc bằng cách để khoảng trắng giữa các id như `!!kenh them id1 id2 id3`...*
</details>

<br>

<details open>
    <summary><strong>4. Đặt Tin nhắn | Nội dung cần gửi.</strong></summary>
    
```diff
!!tinnhan chinhsua NỘI_DUNG_TIN_NHẮN
```
</details>

<br>

<details open>
    <summary><strong>[Tùy chọn] 5. Đặt Hình ảnh làm tệp đính kèm.</strong></summary>
    
```diff
!!dinhkem chinhsua (+ tải lên hình ảnh cùng lúc đồng thời với việc gửi lệnh)
```
*Lưu ý: Cả hai hành động phải được thực hiện cùng lúc.*
<br>
*Lưu ý 2: Tệp đính kèm chỉ chấp nhận hình ảnh có các định dạng sau: `png`, `jpg`, `jpeg`, `gif`, `webp`.*
</details>

<br>

<details open>
    <summary><strong>6. Bật Thư mục | Đã thiết lập xong, hãy bật chế độ tự động.</strong></summary>
    
```diff
!!thumuc bat
```
</details>

<hr>

Sau những bước này, bạn đã hoàn thành việc thiết lập tự động hóa để lặp lại tin nhắn.

Từ giờ, bạn có thể gõ `!!danhsach` để xem thời gian gửi tin nhắn sắp tới.

> **Lưu ý: Trước khi bạn tiếp tục thực hiện bất kỳ bước nào ở trên để tạo thêm thư mục, bạn nên hiểu cách thư mục hoạt động trên nhiều kênh bằng cách đọc [System Handler (Hiệu Chỉnh Hệ Thống)](SystemHandler.md).**

### Vậy nếu bạn đã thành thạo tất cả những điều trên, hãy đến [Full Commands (Lệnh Đầy Đủ)](FullCommands.md) để đọc thêm các lệnh nâng cao/đầy đủ.
