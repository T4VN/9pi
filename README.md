# 9pi Hub — Nice Picture · by T4VN

**9pi Hub** là ứng dụng chính của bộ sản phẩm 9pi: bạn chỉ cần tải **duy nhất
Hub**, sau đó cài thêm các app mong muốn (9pi-Select, 9pi-Color, 9pi-Frame,
9pi-Filter, 9pi-Relight, 9pi-Export) ngay **bên trong Hub** — bấm nút, tự tải
và cài đặt. Toàn bộ làm việc qua **project** chung: chọn ảnh → chỉnh màu →
dựng khung → làm đẹp → đổi ánh sáng → xuất file.

---

## 1. Bắt đầu

1. Tải bản cài đặt cho hệ điều hành của bạn từ trang Releases
   (`9pi-Hub-Setup-v<phiên-bản>-win64.exe` cho Windows, `.dmg` cho macOS,
   `.zip` cho Linux), hoặc tải zip và giải nén:

```
9pi-Hub\
├── 9pi-Hub.exe      ← bấm đúp để mở
├── apps\            ← các app cài thêm nằm ở đây
└── models\          ← model AI dùng chung (tải 1 lần, mọi app dùng)
```

2. Mở Hub — màn hình loading dạng **dialog nhỏ giữa nền tối**: không thể thu
   phóng hay tắt nhầm trong lúc khởi động; nếu thiếu app mặc định, Hub tự tải
   và cài **9pi-Select + 9pi-Export** ngay tại đó, xong tự vào tab PROJECTS.

3. Các app trong Hub (⚙ Cài đặt):

| App | Chức năng |
|---|---|
| 9pi-Select | AI lọc chọn ảnh đẹp: nét, mắt mở, cảm xúc, thẩm mỹ |
| 9pi-Color | Chỉnh màu hàng loạt, học gu màu riêng của studio |
| 9pi-Frame | Dựng khung: crop, xoay, lật — kéo thả trực tiếp trên ảnh |
| 9pi-Filter | Làm đẹp da & khuôn mặt: mịn da, trang điểm, nét |
| 9pi-Relight | Đổi hướng & không khí ánh sáng bằng AI |
| 9pi-Export | Render đúng tham số từng ảnh, xuất JPEG hàng loạt |

Mọi app đều chạy **nhúng trong Hub** qua các tab dưới màn hình — không cần mở
cửa sổ riêng.

## 2. Project — làm việc theo bộ ảnh

- **＋ New Project**: đặt tên + chọn thư mục ảnh (lấy cả thư mục con nếu muốn).
- **Thêm ảnh vào project**: nút **⬇ Thêm ảnh** nằm giữa, ngay trên lưới ảnh
  (project rỗng cũng có nút riêng). Hai cách:
  - **Chọn từng ảnh…** — chọn nhiều file cùng lúc;
  - **Chọn thư mục…** — nhập cả thư mục, tự bỏ qua ảnh đã có.
- **Pin project**: menu **⋯** → Pin — project ghim có **icon ghim màu cam** và
  luôn nằm đầu danh sách.
- Kéo thả để sắp xếp thứ tự, đổi tên, xoá (ảnh gốc không bị xoá).
- **Responsive**: thu nhỏ cửa sổ — sidebar tự thu gọn (nút ❮/❯ mở lại), thanh
  công cụ tự gọn; mọi nút vẫn thao tác được.

## 3. Models AI dùng chung — tải 1 lần

9pi-Select (phân tích) và 9pi-Relight (SD runtime) cần models. Trong
⚙ Cài đặt có dòng **"Models AI dùng chung"**:

- Bấm **Tải ~330MB** → tiến độ hiện ngay tại chỗ (tên file + MB).
- Models nằm trong `models\` — mọi app cài trong Hub **tự dùng đúng thư mục
  này**, không tải lại.

## 4. Kiểm tra cập nhật

⚙ Cài đặt → **Kiểm tra cập nhật**: nếu có phiên bản mới, hộp thoại hiện kèm
**nút tải file cài đặt đúng hệ điều hành** — file về thư mục Downloads và
thư mục chứa file tự mở để bạn chạy cài đặt. Bấm "Để sau" thì phiên bản đó
sẽ không hỏi lại (đến khi có bản mới hơn).

## 5. Quy trình làm việc

1. **PROJECTS**: tạo project, thêm ảnh.
2. **SELECT**: AI phân tích và đề xuất ảnh đẹp — tick chọn.
3. **COLOR**: chỉnh màu theo style có sẵn hoặc tự tinh chỉnh theo từng ảnh.
4. **FRAME**: crop, xoay, lật — kéo thả trực tiếp trên preview, lăn chuột zoom.
5. **FILTER**: làm mịn da, trang điểm theo vùng khuôn mặt AI nhận diện.
6. **RELIGHT**: đổi hướng sáng / không khí ánh sáng (GPU nhanh hơn nhiều).
7. **EXPORT**: render đúng tham số từng ảnh, xuất JPEG hàng loạt.

Ảnh gốc không bao giờ bị ghi đè; mọi thứ chạy trên máy bạn.

## 6. Cài app thủ công (không qua nút Cài đặt)

Tải zip app từ Releases, giải nén sao cho được:

```
9pi-Hub\apps\9pi-Select\9pi-Select.exe
9pi-Hub\apps\9pi-Color\9pi-Color.exe
```

Hub tự nhận diện app mới lần mở sau.

## 7. Gỡ lỗi nhanh

- Nút Cài đặt báo lỗi? Kiểm tra mạng; hoặc tải zip app từ Releases và
  làm theo mục 6.
- App mặc định cài thất bại lúc khởi động? Vào lại sau khi có mạng — Hub tự
  thử lại, hoặc cài tay theo mục 6.
- Chạy Hub chế độ web: `9pi-Hub.exe --no-window` rồi mở
  `http://localhost:8760`.

---

9pi Hub · Nice Picture · **by T4VN**
