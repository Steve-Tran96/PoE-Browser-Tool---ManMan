# PoE Browser Tool - ManMan

## 🛠️ Cài đặt & Yêu cầu
1.  **Yêu cầu hệ thống:**
    * Windows 10/11 (64-bit).
    * .NET Framework 4.7.2 trở lên.
2.  **Cài đặt:**
    * Tải file `.exe` về máy.
    * Tạo thư mục `Images` cùng cấp với file exe để chứa ảnh mẫu (nếu dùng tính năng FindImage).
    * Chạy phần mềm dưới quyền **Administrator** (Run as Admin) để đảm bảo phím tắt hoạt động ổn định.

⚠️ YÊU CẦU BẮT BUỘC (Đọc kỹ trước khi dùng)
    Ngôn ngữ Game: Chuyển sang Tiếng Anh (English) để tool đọc được chỉ số (Mod).
    Chế độ màn hình: Nên để Windowed hoặc Windowed Borderless.
    Vị trí Inventory: Không thay đổi độ phân giải hoặc di chuyển cửa sổ game sau khi đã lưu toạ độ các slot.

HƯỚNG DẪN SỬ DỤNG AUTO ROLL MAP (PATH OF EXILE)
1. CHUẨN BỊ IN-GAME
    Bước 1: Mở rương (Stash) hoặc túi đồ (Inventory).
    Bước 2: Xếp các Map cần roll vào 30 ô đầu tiên của Inventory (hoặc số lượng ô bạn đã cài đặt).
    Bước 3: Chuẩn bị đủ Currency (Chaos Orb, Alchemy Orb...) trong Inventory.
2. Để tránh bị mất Currency hoặc game hiểu nhầm lệnh, hãy làm chính xác theo thứ tự sau:
    Bước 1: Bật Tool và Game song song.
    Bước 2: Cấu hình các Mod cần tìm (Ví dụ: Tránh "Reflect Physical", tìm "Pack Size > 20%" hoặc dùng regex).
    Bước 3: Trong game, Click Chuột Phải vào chồng Currency bạn muốn dùng (ví dụ Chaos Orb) để con trỏ chuột chuyển sang trạng thái "đang cầm Currency".
        💡 Lưu ý: Bạn phải để con trỏ chuột dính Currency TRƯỚC khi bấm nút Start.
    Bước 4: Bấm phím tắt F2 (hoặc nút Start trên Tool) để bắt đầu.
3. CÁC TÍNH NĂNG AN TOÀN (ANTI-BAN)
Tool được tích hợp công nghệ Humanizer để giảm thiểu rủi ro bị quét:
    Delay ngẫu nhiên: Không bao giờ click đều chằn chặn (VD: lúc chờ 200ms, lúc 350ms...).
    Mô phỏng thao tác tay: Click chuột có độ trễ giữa lúc nhấn xuống và nhả ra.
    Cơ chế Retry: Nếu mạng lag hoặc chưa hiện thông tin Map, Tool sẽ kiên nhẫn thử đọc lại thay vì spam click liên tục.

## 📖 Giới thiệu
Macro Tool - ManMan là một phần mềm tự động hóa (Automation Tool) mã nguồn mở được viết bằng C# (Windows Forms).
Tool cho phép người dùng tạo các kịch bản (Macro) phức tạp dựa trên hình ảnh, màu sắc pixel và logic điều kiện để thực hiện các tác vụ lặp đi lặp lại trên Windows, đặc biệt tối ưu cho tựa game **Path of Exile**.

## 🚀 Tính năng nổi bật
* **Smart Interaction:**
    * `HumanMouse`: Di chuyển chuột cong, ngẫu nhiên tốc độ để mô phỏng thao tác người thật.
    * `Smart Keyboard`: Hỗ trợ gõ phím thông minh, tự động xử lý các phím bổ trợ (Shift/Ctrl) để tránh xung đột (Ví dụ: `Shift + Ctrl + C`).
* **Image & Color Recognition:**
    * `FindImage`: Tự động tìm và click vào hình ảnh mẫu trên màn hình (Hỗ trợ Loot đồ, Login, Check trạng thái).
    * `IfColor`: Kiểm tra màu sắc pixel tại tọa độ chỉ định.
* **Advanced Logic:**
    * Hỗ trợ vòng lặp (`Loop`), Điều kiện (`If/Else`), và biểu thức toán học.
    * `RegexExtract`: Trích xuất dữ liệu số từ Clipboard (Dùng để check chỉ số item trong PoE).
* **Safety Features:**
    * Nút **STOP (F11)**: Dừng khẩn cấp và nhả mọi phím đang bị kẹt.
    * Nút **PAUSE (F10)**: Tạm dừng kịch bản để người dùng thao tác tay.

## 📝 Hướng dẫn sử dụng nhanh
1.  Mở Tool -> Chọn cửa sổ Game/Ứng dụng cần chạy.
2.  Nhập kịch bản (Action) vào lưới hoặc dùng chức năng **REC** để ghi lại thao tác.
3.  Nhấn **F9** để Bắt đầu (Start).
4.  Nhấn **F10** để Tạm dừng (Pause).
5.  Nhấn **F11** để Dừng hẳn (Stop/Kill Switch).

---
## ⚠️ MIỄN TRỪ TRÁCH NHIỆM (DISCLAIMER)
Phần mềm này được phát triển với mục đích **nghiên cứu học tập lập trình** (Educational Purposes Only). Tác giả không chịu trách nhiệm cho bất kỳ thiệt hại nào gây ra bởi việc sử dụng phần mềm này, bao gồm nhưng không giới hạn ở:
* Mất mát dữ liệu, lỗi hệ điều hành.
* **Khóa tài khoản (Ban/Lock Account)** trong các trò chơi trực tuyến.
* Vi phạm quy định của nhà phát hành game.

**Người dùng tự chịu hoàn toàn rủi ro khi sử dụng.**
