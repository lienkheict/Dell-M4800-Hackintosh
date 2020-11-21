# Cập nhập OpenCore
 
Để cập nhập phiên bản OpenCore mới nhất bạn có thể thực hiện theo bước sau
1. Truy cập vào địa chỉ [OpenCorePkg's releases](https://github.com/acidanthera/OpenCorePkg/releases/) tải về phiên bản mới nhất của OpenCore
2. Giải nén tệp OpenCore vừa tải về
3. Mount phân vùng EFI
- Sử dụng ứng dụng ứng dụng [OpenCore Configurator](https://mackie100projects.altervista.org/opencore-configurator/) để mount phân vùng EFI của bạn
- Mở phân vùng EFI bạn vừa Mount ra và tiến hành bước tiếp theo
4. Thay thế tệp tin OpenCore mới nhất vào phân vùng EFI
- Thay thế một vài tệp tin giải nén ở bước `2` theo đúng đường dẫn như bên dưới
  - `EFI/BOOT/BOOTx64.efi`
  - `EFI/OC/OpenCore.efi`
  - `EFI/OC/Drivers/OpenRuntime` Tệp này quan trọng nếu không thay OpenCore sẽ không hoạt động được
- Xem hình để thấy được vị trí các tệp tin cần thay đổi
  ![Update OpenCore](https://dortania.github.io/OpenCore-Post-Install/assets/img/usb-folder-highlight.319b4d56.png)


![M4800 BigSur](https://github.com/lienkheict/Dell-M4800-Hackintosh/blob/main/Bigsur.png)
