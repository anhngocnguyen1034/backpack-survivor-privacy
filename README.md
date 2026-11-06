# Bag Buddies — Privacy Policy

Trang chính sách quyền riêng tư của trò chơi **Bag Buddies**
(`com.animalheroes.bagbuddies`), song ngữ Việt — Anh.

**Trang đã xuất bản:** https://anhngocnguyen1034.github.io/bag-buddies-privacy/

URL này dùng để điền vào mục *Privacy Policy* trên Google Play Console.

## Đừng sửa `index.html` bằng tay

Chính sách phải đọc được **ngay trong trò chơi khi không có mạng**, nên chữ gốc nằm trong
`scripts/meta/policy_text.gd` của kho mã trò chơi và được đóng gói thẳng vào APK.
Trang web này **sinh ra từ chính file đó**:

```bash
# trong kho mã trò chơi
~/venv/bin/python -I tools/gen_policy.py ../bag-buddies-privacy
```

Sửa tay `index.html` thì lần sinh sau sẽ ghi đè, và tệ hơn là bản Google đọc sẽ khác bản
người chơi đọc. Luôn sửa ở `policy_text.gd` rồi chạy lại lệnh trên.

Nhớ cập nhật `UPDATED` / `UPDATED_EN` trong `policy_text.gd` mỗi lần đổi nội dung.

## Khi nào bắt buộc phải cập nhật

Trước khi phát hành bất kỳ bản nào có quảng cáo, có SDK phân tích, hoặc có tính năng gửi
dữ liệu ra khỏi máy người chơi.
