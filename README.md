# 9pi Hub — Nice Picture · by T4VN

**9pi Hub** là ứng dụng chính của bộ sản phẩm 9pi: bạn chỉ cần tải **duy nhất
Hub**, sau đó cài thêm các app mong muốn (9pi-Select, 9pi-Color...) ngay
**bên trong Hub** — bấm nút, tự tải và cài đặt.

---

## 1. Bắt đầu

1. Tải `9pi-Hub-v<phiên-bản>-win64.zip` từ trang Releases của repo,
   giải nén được thư mục `9pi-Hub\`:

```
9pi-Hub\
├── 9pi-Hub.exe      ← bấm đúp để mở
├── apps\            ← các app cài thêm nằm ở đây
└── models\          ← model AI dùng chung (tải 1 lần, mọi app dùng)
```

2. Mở Hub — trang chủ hiện các thẻ app:

| Thẻ | Trạng thái | Nút |
|---|---|---|
| 9pi-Select | Chưa cài / Đã cài / Đang chạy | **⬇ Cài đặt** hoặc **Mở app** + **Mở web** |
| 9pi-Color | Chưa cài / Đã cài / Đang chạy | **⬇ Cài đặt** hoặc **Mở app** + **Mở web** |
| 9pi-Edit | Sắp ra mắt | — |

- **⬇ Cài đặt**: tải zip app từ GitHub Releases về, tự giải nén vào
  `apps\` (có thanh tiến độ MB/%).
- **Mở app**: app chưa chạy → bật exe (tự mở cửa sổ riêng). App đang chạy →
  mở lại cửa sổ giao diện, không tạo bản chạy thứ 2.
- **Mở web**: mở giao diện app trong trình duyệt.

## 2. Models AI dùng chung — tải 1 lần

Chỉ **9pi-Select** cần model AI (~330MB). Trên trang chủ Hub có dòng
**"Models AI dùng chung"**:

- Bấm **Tải ~330MB** → tiến độ hiện ngay tại chỗ (tên file + MB).
- Models nằm trong `9pi-Hub\models\` — Select cài trong Hub **tự dùng
  đúng thư mục này**, không tải lại.
- Nếu cài 9pi-Select **độc lập** (không qua Hub): app tự tải models vào
  thư mục `models\` cạnh exe lần phân tích đầu tiên.

## 3. Quy trình Select → Color

1. Mở **9pi-Select**, chọn thư mục ảnh → phân tích → tick chọn ảnh đẹp.
2. Bấm **Gửi sang 9pi-Color** (ngay dưới nút Export ở cạnh trái).
3. 9pi-Color tự mở với đúng các ảnh đã chọn → chọn style / học gu →
   **Export**.

Ảnh gốc không bao giờ bị ghi đè; mọi thứ chạy trên máy bạn.

## 4. Cài app thủ công (không qua nút Cài đặt)

Tải zip app từ Releases, giải nén sao cho được:

```
9pi-Hub\apps\9pi-Select\9pi-Select.exe
9pi-Hub\apps\9pi-Color\9pi-Color.exe
```

Hub tự nhận diện app mới lần mở sau. Hub cũng nhận diện app đặt cạnh nó
(theo layout cũ `9pi-Hub\9pi-Select\9pi-Select\...`).

## 5. Gỡ lỗi nhanh

- Nút Cài đặt báo lỗi? Kiểm tra mạng; hoặc tải zip app từ Releases và
  làm theo mục 4.
- Chạy Hub chế độ web: `9pi-Hub.exe --no-window` rồi mở
  `http://localhost:8760`.

---

9pi Hub · Nice Picture · **by T4VN**
