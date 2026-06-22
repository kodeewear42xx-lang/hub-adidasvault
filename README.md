# 👟 ADIDAS VAULT · Store Phú Quốc

Website bán giày & dép **adidas chính hãng** (tiếp thị liên kết Shopee) — bộ sưu tập mới nhất, thời tiết & giờ Phú Quốc trực tiếp, đồng hành **World Cup 2026**.

🔖 `#kodeewear20xx` · Phú Quốc, Kiên Giang

---

## ✨ Tính năng

- **97 sản phẩm** giày & dép, lọc theo nhóm / giới tính, tìm kiếm, sắp xếp giá. Nút "Mua trên Shopee" gắn link affiliate.
- **Ảnh sản phẩm 3D** vẽ bằng SVG (gradient, bóng đổ) — không cần file ảnh, không vỡ. Mã nào có ảnh thật sẽ tự ưu tiên hiển thị.
- **Đồng hồ vòng** + **thời tiết Phú Quốc** trực tiếp (Open-Meteo, miễn phí, không cần key).
- **World Cup 2026 LIVE**: kết quả tự cập nhật từ ESPN (logo đội thật), 1 trận nổi bật + các trận live/vừa đá/sắp đá. Có fallback khi mất mạng.
- **Đánh giá khách hàng**, **Flash Sale đếm ngược**, **Đối tác & tài trợ**.
- Giao diện tối tông slate + accent lime, logo 3 sọc đỏ/vàng/xanh, hiệu ứng fade-in tinh tế.

---

## 🚀 Cách deploy (GitHub Pages)

1. Tạo repo (hoặc dùng repo sẵn có).
2. Up file **`index.html`** vào nhánh `main`.
3. Vào **Settings → Pages → Source**: chọn `main` / `root` → **Save**.
4. Đợi ~1 phút, web chạy tại `https://<tên-user>.github.io/<tên-repo>/`.

> Toàn bộ web nằm trong 1 file `index.html` duy nhất — không cần build, không cần thư viện cài đặt.

---

## 🖼️ Thêm ảnh sản phẩm thật

Có 2 cách, mã nào chưa có ảnh thì giữ hình 3D minh hoạ:

**Cách A — bỏ file vào repo:** tạo thư mục `images/`, đặt tên ảnh **theo mã sản phẩm**, đuôi `.jpg`:
```
images/FY6680.jpg
images/KZ6848.jpg
```

**Cách B — gắn link/base64 trong code:** mở `index.html`, tìm biến `IMAGES` và thêm dòng:
```js
const IMAGES = {
  "FY6680":"https://link-anh-truc-tiep.jpg",
  "KZ6848":"data:image/jpeg;base64,....",
};
```

---

## ✏️ Chỉnh nội dung nhanh (trong `index.html`)

| Muốn sửa | Tìm biến / khối |
|---|---|
| Ảnh sản phẩm | `const IMAGES` |
| Đánh giá khách hàng | `const REVIEWS` |
| Tin & nhận định World Cup | `const WCNEWS` |
| Kết quả dự phòng World Cup | `const WC_FALLBACK` |
| Đối tác & tài trợ | khối `<!-- PARTNERS -->` |
| Toạ độ thời tiết | `latitude=10.227&longitude=103.967` |

---

## 🤝 Đối tác & tài trợ

- [Vivu Phú Quốc](https://vaultadidas-collab.github.io/vivuphuquoc-chill/) — du lịch & khám phá
- [Sony Hub](https://vaultadidas-collab.github.io/kodeeboyzz-SONYHuB/) — Sony nét mượt, chính hãng
- [Kodeewear20xx Hub](https://vaultadidas-collab.github.io/Kodeewear20xx-hub/) — quần áo authentic

---

## ⚠️ Ghi chú

- Trang theo hình thức **tiếp thị liên kết (affiliate)** — giá, tồn kho, thanh toán do **Shopee** xử lý.
- Phần đánh giá hiện là **mẫu**, nên thay bằng đánh giá thật từ Shopee.
- Dữ liệu World Cup mang tính tham khảo — xem chính thức tại FIFA.com.

© 2026 ADIDAS VAULT · made for JoinTon · `#kodeewear20xx`
