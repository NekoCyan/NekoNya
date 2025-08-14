# Discord Tool - Black Market Tool (Business Market Tool)

_Lệnh Người Dùng - Lệnh Nâng Cao/Đầy Đủ_

<hr>

Trước khi đọc phần dưới đây, nếu bạn là người mới/mới bắt đầu với công cụ này, tốt hơn hết hãy đọc [Beginner Commands](BeginnerCommands.md) trước.

<hr>

Mục lục

-   [1. Hướng dẫn lệnh Thư mục](#1-hướng-dẫn-lệnh-thư-mục)
-   [2. Hướng dẫn lệnh Thời gian](#2-hướng-dẫn-lệnh-thời-gian)
-   [3. Hướng dẫn lệnh Kênh](#3-hướng-dẫn-lệnh-kênh)
-   [4. Hướng dẫn lệnh Tin nhắn](#4-hướng-dẫn-lệnh-tin-nhắn)
-   [5. Hướng dẫn lệnh Đính kèm](#5-hướng-dẫn-lệnh-đính-kèm)
-   [Chủ động gọi tên thư mục trong lệnh (Thư mục động)](#chủ-động-gọi-tên-thư-mục-trong-lệnh-thư-mục-động)

<hr>

## 1. Hướng dẫn lệnh Thư mục

> Dùng để xử lý thời gian, kênh mà bạn đã thêm, tin nhắn mà bạn đã đặt và nhiều mục đích khác cho việc tự động.

_Nhấp vào từng phần bên dưới để mở rộng và xem chi tiết._

<details>
    <summary><strong>Chọn thư mục | Vì bạn có thể thêm nhiều thư mục, nên chúng ta sẽ điều khiển thư mục cụ thể bằng cách chọn nó.</strong></summary>
    
```diff
!!thumuc chon TÊN_THƯ_MỤC
```
</details>

<details>
    <summary><strong>Tạo thư mục | Tạo một thư mục mới và tự động chọn nó (Tối đa 25 thư mục có thể được tạo).</strong></summary>
    
```diff
!!thumuc them TÊN_THƯ_MỤC
```
</details>

<details>
    <summary><strong>Đổi tên thư mục.</strong></summary>
    
```diff
!!thumuc doiten TÊN_THƯ_MỤC_CŨ TÊN_THƯ_MỤC_MỚI
```
</details>

<details>
    <summary><strong>Xóa thư mục.</strong></summary>
    
```diff
!!thumuc xoa TÊN_THƯ_MỤC
```
</details>

<details>
    <summary><strong>Hiển thị thư mục | hiển thị các thư mục mà bạn đã thêm trước đó.</strong></summary>
    
```diff
!!thumuc hienthi
```
</details>

<details>
    <summary><strong>Bật thư mục | Kích hoạt chức năng để kích hoạt tự động hóa.</strong></summary>
    
```diff
!!thumuc bat
```
</details>

<details>
    <summary><strong>Tắt thư mục | Vô hiệu hóa/Dừng chức năng.</strong></summary>
    
```diff
!!thumuc tat
```
</details>

<details>
    <summary><strong>Cài đặt lại thư mục | Xóa hoàn toàn tất cả thư mục cùng lúc.</strong></summary>
    
```diff
!!thumuc caidatlai
```
</details>

## 2. Hướng dẫn lệnh Thời gian

_Nhấp vào từng phần bên dưới để mở rộng và xem chi tiết._

<details>
    <summary><strong>Đặt thời gian | Đặt thời gian cho việc lặp lại tin nhắn.</strong></summary>
    
```diff
!!thoigian chinhsua THỜI_GIAN
```
Timer phải có định dạng `1s`, `2m`, `3h`, `4d` (tức là 1 giây, 2 phút, 3 giờ, 4 ngày).
<br>
Ví dụ: `!!thoigian chinhsua 5m` # Đặt thời gian của thư mục thành 5 phút
</details>

## 3. Hướng dẫn lệnh Kênh

_Nhấp vào từng phần bên dưới để mở rộng và xem chi tiết._

<details>
    <summary><strong>Thêm kênh.</strong></summary>
    
```diff
!!kenh them ID_CHANNEL
```
*Bạn có thể thêm nhiều kênh cùng lúc bằng cách để khoảng trắng giữa các id như `!!kenh them id1 id2 id3`...*
</details>

<details>
    <summary><strong>Hiển thị kênh | Hiển thị tất cả kênh (dưới dạng mention) mà bạn đã thêm vào thư mục.</strong></summary>
    
```diff
!!kenh hienthi
```
</details>

<details>
    <summary><strong>Hiển thị id kênh | Hiển thị tất cả kênh (chỉ id) mà bạn đã thêm vào thư mục.</strong></summary>
    
```diff
!!kenh hienthiid
```
</details>

<details>
    <summary><strong>Xóa kênh.</strong></summary>
    
```diff
!!kenh xoa ID_CHANNEL
```
*Bạn có thể xóa nhiều kênh cùng lúc bằng cách để khoảng trắng giữa các id như `!!kenh xoa id1 id2 id3`...*
<br>
*Nếu bạn xóa một kênh không có trong thư mục hiện tại, hệ thống sẽ mở rộng/khắp tất cả thư mục và xóa nó nếu tìm thấy.*
</details>

<details>
    <summary><strong>Cài đặt lại kênh | Xóa hoàn toàn tất cả kênh cùng lúc trong thư mục.</strong></summary>
    
```diff
!!kenh caidatlai
```
</details>

## 4. Hướng dẫn lệnh Tin nhắn

_Nhấp vào từng phần bên dưới để mở rộng và xem chi tiết._

<details>
    <summary><strong>Đặt tin nhắn | Đặt nội dung tin nhắn dùng để gửi.</strong></summary>
    
```diff
!!tinnhan chinhsua NỘI_DUNG_TIN_NHẮN
```

Slash Command được hỗ trợ nhưng chỉ thực hiện lệnh đơn như `/sound` chứ không phải như `/sound on`.

```diff
!!tinnhan chinhsua /{BOT_ID} {LỆNH_CỦA_BOT}
```

Ví dụ lệnh: Muốn thực hiện lệnh **`daily`** trên bot có id là **`123`**, đầu vào sẽ là `!!tinnhan chinhsua /123 daily`.

</details>

<details>
    <summary><strong>Hiển thị tin nhắn | Hiển thị nội dung tin nhắn mà bạn đã đặt.</strong></summary>
    
```diff
!!tinnhan hienthi
```
</details>

## 5. Hướng dẫn lệnh Đính kèm

<details>
    <summary><strong>Đặt đính kèm | Đặt ảnh đính kèm cho việc gửi cùng lúc với nội dung tin nhắn.</strong></summary>
    
```diff
!!dinhkem chinhsua (+ tải lên hình ảnh cùng lúc đồng thời với việc gửi lệnh)
```
</details>

<details>
    <summary><strong>Hiển thị đính kèm | Hiển thị các đính kèm mà bạn đã đặt.</strong></summary>
    
```diff
!!dinhkem hienthi
```

Nó sẽ hiển thị đường link thay vì tải lên. Nhưng đừng lo lắng, nó sẽ được tải lên ở kênh mà bạn đã chỉnh cùng với nội dung tin nhắn.

</details>

<details>
    <summary><strong>Cài đặt lại đính kèm | Xóa hoàn toàn tất cả đính kèm cùng lúc trong thư mục.</strong></summary>
    
```diff
!!dinhkem caidatlai
```
</details>

## Chủ động gọi tên thư mục trong lệnh (Thư mục động)

Một số lệnh được hỗ trợ để gọi trực tiếp trên lệnh (bằng cách sử dụng dấu trừ `-`) mà không cần phải chọn thư mục trước.

#### Ví dụ, nếu bạn muốn bật một thư mục, bạn phải thực hiện hai lệnh dưới đây:

```diff
!!thumuc chon TÊN_THƯ_MỤC
!!thumuc bat
```

Nhưng từ giờ, bạn có thể đơn giản thực hiện trong một lệnh để chạy một hoặc nhiều thư mục (FOLDER) cùng lúc:

```diff
!!thumuc bat -FOLDER1 -FOLDER2 -FOLDER3 -FOLDER_N+1...
```

Chúng tôi cũng hỗ trợ từ khóa `tatca` để thực hiện lệnh cho tất cả thư mục cùng lúc:

```diff
!!thumuc bat -tatca
```

#### Ví dụ với lệnh đặt tin nhắn:

```diff
!!tinnhan chinhsua -FOLDER1 -FOLDER2 -FOLDER3 -FOLDER_N+1... NỘI_DUNG_TIN_NHẮN
```

#### Ví dụ với lệnh thêm kênh:

```diff
!!kenh them -FOLDER1 id1 id2 id3
```

> **Lưu ý**: Các thư mục động trong lệnh phải được đặt trước khi đặt bất kỳ giá trị nào (như nội dung tin nhắn, id kênh, v.v.).

## Một số lệnh liên quan đến cài đặt lại, giới hạn chỉ thực hiện cho một thư mục sẽ bị hạn chế sử dụng gọi thư mục động, bạn có thể thử một số nếu có bug nào, phản hồi cho tôi, Neko ~
