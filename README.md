# GRUB with efidriver v2 patch

本專案基於 [GNU GRUB](https://www.gnu.org/software/grub/) (GPLv3)，
並套用由 Nikita Travkin 提交至 grub-devel 郵件列表的 efidriver v2 patch
(base-commit: 9c34d56c2dafcd2737db0e3e49df63bce4d8b504)。

## 授權
本專案遵循 GPLv3 授權。使用者可自由使用、修改、再散佈，
但若散佈 binary，必須同時提供對應的原始碼與修改。

## 修改內容
- 套用 efidriver v2 patch
- 編譯成 `grubx64.efi`，包含以下模組：
  - efidriver, chainloader
  - part_gpt, part_msdos
  - fat, ext2
  - normal, linux, efi_gop, efi_uga

## 注意事項
此 binary 僅供測試用途。若要公開散佈，請一併提供原始碼與 patch。
