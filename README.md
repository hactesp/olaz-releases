# Olaz — bản phát hành / Releases

**Olaz** là ứng dụng Zalo gốc cho macOS, viết bằng Rust. Repo này chỉ chứa **các bản tải về**.
*Olaz is a native macOS Zalo client written in Rust. This repository only hosts downloads.*

> [!IMPORTANT]
> **Dự án không chính thức, không liên kết với hay được VNG Corporation bảo trợ.** "Zalo" là nhãn hiệu của VNG.
> Dùng ứng dụng không chính thức có thể trái điều khoản dịch vụ của Zalo: bạn tự chịu rủi ro, chỉ dùng với
> tài khoản của chính mình.
> *Unofficial, not affiliated with or endorsed by VNG. Use at your own risk with your own account.*

## Tải về

Vào trang **[Releases](../../releases)** và tải `Olaz-<phiên bản>.dmg`.

Yêu cầu: macOS 11 trở lên, Mac Apple Silicon (arm64), tài khoản Zalo và Zalo trên điện thoại để quét QR.

## Cài đặt

1. Mở file `.dmg`, kéo **Olaz** vào **Applications**.
2. Bản này **chưa được Apple công chứng**. Lần đầu: bấm chuột phải vào Olaz → **Open** → **Open**.
   Nếu macOS vẫn chặn: *System Settings → Privacy & Security → Open Anyway*, hoặc chạy
   `xattr -dr com.apple.quarantine /Applications/Olaz.app`.
3. Lần đầu mở, Olaz tải bộ cài Zalo PC chính thức từ VNG (~270 MB), kiểm tra chữ ký của VNG rồi mới dùng.
4. Cho phép thông báo khi được hỏi. macOS có thể hỏi quyền Keychain: chọn **Always Allow** (Olaz lưu khóa mã
   hóa phiên đăng nhập ở đó). Micro/camera được hỏi ở cuộc gọi đầu tiên.
5. Quét mã QR bằng Zalo trên điện thoại.

Zalo chỉ cho **một phiên máy tính cho mỗi tài khoản**: nếu Zalo PC chính thức đang chạy, hãy thoát nó trước.

## Kiểm tra tệp tải về

Mỗi bản phát hành ghi SHA-256 của từng tệp. Kiểm tra bằng `shasum -a 256 Olaz-<phiên bản>.dmg`.

## Báo lỗi

Mở một [issue](../../issues) (đừng đăng ảnh chụp có tin nhắn hoặc thông tin cá nhân).

## Giấy phép / Licence

Olaz dựa trên phần mềm GPL-3.0 (zalo-swift-re và libsignal-protocol-javascript). Theo GPL-3.0, bạn có thể
**yêu cầu mã nguồn** của bản bạn đã tải: mở một issue ở đây để được cung cấp.
*Olaz is based on GPL-3.0 software; the corresponding source code is available on request via an issue.*
