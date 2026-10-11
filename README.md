# TOEIC Garden

Website ôn từ vựng bằng ReactJS 19 và Vite. Giao diện tiếng Việt, dùng trên máy tính và điện thoại.

## Chạy ở máy của bạn

```bash
npm ci
npm run dev
```

## Tạo bản phát hành

```bash
npm run build
npm run preview
```

## Nội dung và chức năng

- 5.031 mục từ từ Index của Hackers TOEIC Vocabulary, chia theo 30 ngày và số trang được chỉ dẫn trong Index.
- 313 nghĩa ngắn được biên soạn để lật thẻ và làm trắc nghiệm; các mục còn lại mở ảnh trang giải nghĩa trong bản sách người dùng có tại máy.
- Lật thẻ, trộn thứ tự, phát âm qua tính năng của trình duyệt, đánh dấu đã nhớ/cần ôn và lưu từ.
- Tìm kiếm tiếng Anh và nghĩa tiếng Việt đã có; sao lưu/khôi phục tiến độ bằng JSON.
- Tiến độ lưu riêng trong localStorage của trình duyệt; chưa đồng bộ giữa thiết bị.

`src/main.jsx` chứa các component React và logic ôn tập. `src/style.css` và `src/additional.css` chứa giao diện responsive. `public/data.js` chứa bộ từ và số trang; `public/pages/` chứa ảnh trang được dùng để đối chiếu.

Danh sách được nhận dạng từ tài liệu Index dạng ảnh; đã sửa các lỗi thấy được trong quá trình kiểm tra, nhưng chưa đối chiếu thủ công từng mục. Vì vậy, trang sách được giữ lại làm nguồn xác nhận cách viết, nghĩa và cách dùng.

Một số trang 301–311 không có trong bản scan. Các mục từ ở các trang này đã được bổ sung nghĩa ngắn. Số mục trong Index không tương đương số lần xuất hiện của từ/cụm từ trong toàn bộ sách.
