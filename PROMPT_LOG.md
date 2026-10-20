# NHẬT KÝ PROMPT ENGINEERING (VIBE CODING LOG)

- **Họ và tên:** Trần Thị Quỳnh Như
- **MSSV:** 125000162
- **Tên đề tài Website:** Portfolio cá nhân – Trần Thị Quỳnh Như
- **Công cụ AI đã sử dụng:** Google Antigravity (quá trình xây dựng), ChatGPT (hỗ trợ kiểm tra và chỉnh sửa GitHub)

> Nhật ký cần giữ lại **đúng nguyên văn các Prompt thực sự đã gửi**. Những đoạn trong ngoặc vuông dưới đây chờ sinh viên dán từ lịch sử hội thoại với AI, không phải Prompt được AI tự bịa.

## 1. Yêu cầu ban đầu (System/Initial Prompt)

**Prompt khởi tạo đã dùng:**

> [DÁN NGUYÊN VĂN PROMPT KHỞI TẠO ĐÃ GỬI VÀO GOOGLE ANTIGRAVITY]

**Ý tưởng đã triển khai:** Website Portfolio giới thiệu bản thân, kỹ năng, dự án và thông tin liên hệ; phong cách pastel. Cấu trúc được chia thành các section để dễ xây dựng và kiểm tra.

## 2. Quá trình tinh chỉnh & Giải quyết sự cố (Iteration Iterations)

### Lần 1: Dựng khung Semantic HTML & CSS Variable

- **Prompt đã dùng:**
  > [DÁN PROMPT THỰC TẾ YÊU CẦU ANTIGRAVITY TẠO HTML/CSS]
- **Kết quả AI tạo ra:** Có file `index.html` chứa `header`, `nav`, `main`, nhiều `section` và `footer`. File `style.css` có `:root`, dùng `var(...)`, Flexbox, Grid và media query responsive.
- **Nhận xét & tinh chỉnh của SV:** Giao diện được chia thành các khu vực dễ theo dõi. Khi rà soát, mình chú ý bố cục trên điện thoại, khoảng cách giữa các thẻ và việc dùng HTML có ngữ nghĩa.
- **Prompt tinh chỉnh (nếu đã thực sự gửi):**
  > [DÁN PROMPT TINH CHỈNH THỰC TẾ HOẶC GHI KHÔNG CÓ]

### Lần 2: Tích hợp Animate.css & hiệu ứng cuộn

- **Prompt đã dùng:**
  > [DÁN PROMPT THỰC TẾ YÊU CẦU HIỆU ỨNG]
- **Kết quả kiểm tra:** Tiêu đề trang chủ có Animate.css; các thành phần nội dung được gắn `data-aos` trong bản đầu.
- **Thách thức gặp phải:** Đề PDF có yêu cầu AOS, trong khi giảng viên cấm sử dụng JavaScript. AOS chính thức cần JavaScript để khởi tạo nên không thể đồng thời thỏa mãn cả hai yêu cầu bằng AOS gốc.
- **Cách sửa Prompt (Debug prompt):**
  > [DÁN PROMPT THỰC TẾ YÊU CẦU BỎ JAVASCRIPT VÀ CHUYỂN HIỆU ỨNG SANG CSS]
- **Kết quả sau tinh chỉnh:** Bỏ các thẻ `script` và phần tải AOS gốc; dùng CSS `@keyframes`, `animation-timeline: view()`, `:hover` và `:focus-visible`. Giao diện vẫn có hiệu ứng, đồng thời nội dung vẫn hiển thị trên trình duyệt chưa hỗ trợ Scroll-driven Animations.

### Lần 3: Kiểm tra khi triển khai GitHub Pages

- **Vấn đề thực tế:** Ảnh chân dung không hiện do đường dẫn trong HTML không khớp vị trí file ảnh trong Repository.
- **Cách giải quyết:** Kiểm tra đường dẫn ảnh, rồi nhúng dữ liệu ảnh chân dung trực tiếp vào `index.html`. Các file hình dự án dùng đường dẫn tương đối cùng cấp.
- **Kết quả:** Ảnh chân dung đã hiển thị trên GitHub Pages.
- **Prompt/câu hỏi đã dùng để xử lý (nếu cần ghi):**
  > [DÁN NGUYÊN VĂN CÂU HỎI HOẶC PROMPT THỰC TẾ]

## 3. Đánh giá cá nhân về quá trình Vibe Coding

**AI đã giúp bạn tiết kiệm thời gian ở phần nào nhất?**

AI giúp mình dựng khung HTML và CSS nhanh hơn, nhất là phần chia section, viết CSS Variables và bố trí responsive. Nhờ đó mình có thêm thời gian xem lại cách hiển thị và sửa các chỗ chưa hợp lý.

**Bài học rút ra khi đặt câu hỏi (Prompt) cho AI trong thiết kế web?**

Mình thấy cần nêu yêu cầu cụ thể, ví dụ cần những thẻ HTML nào, giao diện ra sao và điều gì bị giới hạn. Không nên chỉ bảo AI làm website đẹp, vì kết quả có thể thiếu tiêu chí của đề. Sau khi AI tạo code, mình vẫn phải mở website, thử thao tác và kiểm tra lại từng mục.

---

**Ghi chú:** Những phần trong ngoặc vuông phải được sinh viên thay bằng lịch sử Prompt thật trước khi coi đây là nhật ký hoàn tất. Không ghi những prompt chưa từng sử dụng.
