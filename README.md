# 📘 Workflow đánh giá README.md trên GitHub bằng n8n

Dự án này cung cấp một **workflow tự động sử dụng n8n** để đánh giá chất lượng file `README.md` của các repository công khai trên GitHub, dựa trên 10 tiêu chí đánh giá phổ biến.

---

## 🚀 Tính năng chính

- 🔎 Tự động lấy nội dung file `README.md` từ các repo trên GitHub
- 🧠 Phân tích nội dung dựa trên các tiêu chí chất lượng
- 📊 Trả về điểm số hoặc bảng đánh giá chi tiết cho từng repo
- 📤 Có thể gửi kết quả qua email, Slack, hoặc lưu trữ vào Airtable/Notion
- 🔁 Hỗ trợ chạy theo lịch hoặc thủ công

---

## ⚙️ Cài đặt

### Bước 1: Clone dự án về máy
git clone https://github.com/ten-ban/readme-evaluator-n8n.git
cd readme-evaluator-n8n
### Bước 2: Nhập workflow vào n8n
Truy cập giao diện n8n của bạn

Nhấn Import và chọn file README_Evaluator_Workflow.json đã cung cấp

### Bước 3: Cấu hình các kết nối (Credentials)
Workflow này sử dụng các dịch vụ:

GitHub API để lấy README

(Tuỳ chọn) OpenAI API hoặc logic nội bộ để phân tích nội dung

(Tuỳ chọn) Gửi kết quả qua Email, Slack, hoặc lưu trữ vào Google Sheets, Airtable, v.v.

Bạn cần thiết lập các kết nối trong phần Settings > Credentials của n8n.

