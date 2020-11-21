# Cập nhập OpenCore
 > Chú ý: Trước khi thực hiện cập nhập phiên bản mới nhất của OpenCore, bạn nên tạo một bản sao lưu phân vùng EFI hiện tại của máy ra USB để phòng trường hợp cập nhập lỗi hoặc không tương thích phiên bản mới máy của bạn.
 
Để cập nhập phiên bản OpenCore mới nhất bạn có thể thực hiện theo bước sau
1. Truy cập vào địa chỉ [OpenCorePkg's releases](https://github.com/acidanthera/OpenCorePkg/releases/) tải về phiên bản mới nhất của OpenCore
2. Giải nén tệp OpenCore vừa tải về
3. Mount phân vùng EFI
- Sử dụng ứng dụng ứng dụng [OpenCore Configurator](https://mackie100projects.altervista.org/opencore-configurator/) để mount phân vùng EFI của bạn

![Mount EFI](https://github.com/lienkheict/Dell-M4800-Hackintosh/blob/main/OpenCore/mount_efi.png)

- Mở phân vùng EFI bạn vừa Mount ra và tiến hành bước tiếp theo
4. Thay thế tệp tin OpenCore mới nhất vào phân vùng EFI
- Thay thế một vài tệp tin giải nén ở bước `2` theo đúng đường dẫn như bên dưới
  - `EFI/BOOT/BOOTx64.efi`
  - `EFI/OC/OpenCore.efi`
  - `EFI/OC/Drivers/OpenRuntime` Tệp này quan trọng nếu không thay OpenCore sẽ không hoạt động được
- Xem hình để thấy được vị trí các tệp tin cần thay đổi
![Update OpenCore](https://dortania.github.io/OpenCore-Post-Install/assets/img/usb-folder-highlight.319b4d56.png)
5. Cập nhập thay đổi trong file config.plist
> Khi cập nhập lên phiên bản OpenCore mới nhất, thường thì sẽ có một một vài thay đổi trong tệp tin config.plist do vậy bạn phải cập nhập lại để máy của bạn có thể khởi chạy hoặc chạy tốt hơn

Để thực hiện bạn có thể sử dụng ứng dụng [OCConfigCompare](https://github.com/corpnewt/OCConfigCompare) để so sánh giữa hai tệp tin 

![Compare plist](https://github.com/lienkheict/Dell-M4800-Hackintosh/blob/main/OpenCore/compare_plist.png)



