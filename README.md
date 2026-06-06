# Git Foundation Practice Repository

## Giới thiệu Repository

Repository này được tạo nhằm thực hành các kiến thức và kỹ năng cơ bản về Git và GitHub trong khuôn khổ khóa học Git Foundation.

Trong quá trình thực hiện, tôi đã áp dụng các thao tác quan trọng như tạo branch, commit, pull request, merge, xử lý conflict và revert commit. Repository cũng đóng vai trò là tài liệu tổng hợp những kiến thức đã học và kinh nghiệm thực hành với Git.

---

# Kiến thức Git cơ bản

## Git là gì?

Git là một hệ thống quản lý phiên bản phân tán (Distributed Version Control System) giúp theo dõi lịch sử thay đổi của mã nguồn và hỗ trợ làm việc nhóm hiệu quả.

## Một số lệnh Git cơ bản

### Kiểm tra trạng thái

```bash
git status
```

### Thêm file vào vùng staging

```bash
git add .
```

### Tạo commit

```bash
git commit -m "Commit message"
```

### Đẩy code lên GitHub

```bash
git push origin main
```

### Cập nhật code từ remote

```bash
git pull origin main
```

### Xem lịch sử commit

```bash
git log --oneline
```

---

# Quy trình làm việc với Git và GitHub

Quy trình làm việc cơ bản:

1. Clone repository từ GitHub về máy.
2. Tạo branch mới để phát triển tính năng.
3. Thực hiện thay đổi mã nguồn.
4. Commit các thay đổi.
5. Push branch lên GitHub.
6. Tạo Pull Request.
7. Review và Merge Pull Request vào nhánh chính.
8. Đồng bộ lại repository.

Quy trình này giúp quản lý thay đổi hiệu quả và hạn chế ảnh hưởng đến nhánh chính.

---

# Hướng dẫn tạo Branch

## Tạo branch mới

```bash
git checkout -b AI
```

Hoặc:

```bash
git branch AI
git checkout AI
```

## Kiểm tra danh sách branch

```bash
git branch
```

## Chuyển branch

```bash
git checkout main
```

## Push branch lên GitHub

```bash
git push origin AI
```

Trong quá trình thực hành, các branch được sử dụng gồm:

* main
* chương
* AI
* K3
* demo

---

# Hướng dẫn Pull Request

Pull Request (PR) được sử dụng để đề xuất hợp nhất thay đổi từ một branch vào branch khác.

Các bước thực hiện:

1. Push branch lên GitHub.
2. Chọn "Compare & Pull Request".
3. Nhập tiêu đề và mô tả.
4. Nhấn "Create Pull Request".
5. Review thay đổi.
6. Chọn "Merge Pull Request".

Lợi ích của Pull Request:

* Kiểm tra mã nguồn trước khi merge.
* Theo dõi lịch sử thay đổi.
* Hỗ trợ làm việc nhóm hiệu quả.

---

# Thực hành Merge Conflict

Merge Conflict xảy ra khi hai branch cùng chỉnh sửa một vị trí trong cùng một file.

## Tình huống thực hành

* Branch demo chỉnh sửa nội dung README.md.
* Branch main cũng chỉnh sửa cùng vị trí đó.
* Khi thực hiện merge, Git phát hiện conflict.

Ví dụ:

```text
<<<<<<< HEAD
Version from main
=======
Version from demo
>>>>>>> demo
```

## Cách xử lý

1. Mở file bị conflict.
2. Chỉnh sửa lại nội dung mong muốn.
3. Xóa các ký hiệu conflict.
4. Lưu file.
5. Commit lại kết quả sau khi resolve.

```bash
git add README.md
git commit -m "Resolve merge conflict"
```

---

# Thực hành Revert Commit

Revert được sử dụng để hoàn tác một commit nhưng vẫn giữ nguyên lịch sử dự án.

## Thực hiện revert

```bash
git revert HEAD
```

Git sẽ tạo một commit mới để đảo ngược các thay đổi trước đó.

Ưu điểm:

* An toàn.
* Không làm mất lịch sử commit.
* Phù hợp khi làm việc nhóm.

---

# Tổng kết các nội dung đã học trong khóa Git Foundation

Sau khi hoàn thành khóa học và thực hành trên repository này, tôi đã nắm được:

* Kiến thức cơ bản về Git và GitHub.
* Cách quản lý mã nguồn bằng Git.
* Tạo và sử dụng branch hiệu quả.
* Thực hiện commit với thông điệp rõ ràng.
* Sử dụng Pull Request trong quy trình phát triển phần mềm.
* Xử lý Merge Conflict.
* Thực hiện Revert và Rollback an toàn.
* Áp dụng GitHub Flow vào quy trình làm việc.
* Các nguyên tắc làm việc an toàn với Git và GitHub.
* Cách kết hợp Git với AI để hỗ trợ phát triển phần mềm hiệu quả.

Repository này là minh chứng cho quá trình học tập và thực hành các kiến thức Git Foundation.
