Nội dung ghi chú githuub
---

# **GitHub Notes**

## **1. Add `.gitignore`**
- Tạo file `.gitignore` để chỉ định các tệp/thư mục không muốn đưa vào Git.
- Ví dụ:
  ```plaintext
  # Bỏ qua tệp tạm của hệ điều hành
  *.DS_Store
  Thumbs.db

  # Bỏ qua tệp biên dịch
  *.exe
  *.class

  # Bỏ qua thư mục node_modules
  node_modules/
  ```

---

## **2. Issues**
- **Chức năng:** Công cụ quản lý công việc trên GitHub.
- **Sử dụng:**
  - Mở **tab Issues** trong repository.
  - Tạo **Issue** mới để mô tả lỗi, tính năng mới, hoặc ý tưởng.
  - Liên kết Issues với Pull Request để quản lý công việc.

---

## **3. Branch và Merge**

### **Lệnh cơ bản với nhánh:**
- **Xem nhánh hiện tại**:  
  ```bash
  git branch
  ```
- **Tạo nhánh mới**:  
  ```bash
  git branch <new_branch>
  ```
- **Chuyển nhánh**:  
  ```bash
  git checkout <branch>
  ```

### **Pull Request (PR):**
- Yêu cầu hợp nhất (merge) một nhánh vào nhánh chính (ví dụ: từ `feature` sang `main`).
- Quy trình:
  1. Tạo PR trong GitHub.
  2. Người khác review code.
  3. Hợp nhất nếu đạt yêu cầu.

### **Merge và Giải quyết xung đột**
1. Khi có xung đột, bạn sẽ thấy đoạn mã như sau:
   ```plaintext
   # tìm kiếm
   <<<<<<< HEAD
   # Nội dung của nhánh hiện tại

   # thêm vào
   =======
   # Nội dung của nhánh main
   >>>>>>> main
   ```
2. Chỉnh sửa mã để kết hợp hoặc chọn phiên bản bạn muốn giữ.
3. Sau đó, đánh dấu đã giải quyết:
   ```bash
   git add <file>
   git commit
   ```

---

## **Tham khảo**
- Video hướng dẫn Git cơ bản:  
  [Git and GitHub for Beginners](https://www.youtube.com/watch?v=oMtzGyAsF2M)

---

