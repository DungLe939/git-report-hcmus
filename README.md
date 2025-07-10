# 1. Tổng quan về Git và GitHub
- Git là gì ?
- Tại sao lại dùng Git?
-  Lịch sử của Git.
- Git Workflow.
- GitHub là gì ?
- GitHub có chức năng g ì?
- Sự khác nhau giữa Git và GitHub.
---
# 2. Các khái niệm

Sau khi bạn đã biết được các khái niệm cũng như là Git và GitHub. Để làm quen với công cụ Git và Github chúng ta có những khái niệm quan trọng như sau.
## 2.1 Repository

**Repository** hay thường được gọi tắt là repo là một khái niệm trung tâm trong Git. Về bản chất, repository là một kho lưu trữ mã nguồn của dự án, nơi chứa toàn bộ tập tin, thư mục và các thông tin liên quan đến lịch sử phát triển phần mềm. Toàn bộ tiến trình làm việc, từ tạo mới, chỉnh sửa, cho đến theo dõi các thay đổi trong dự án đều được ghi nhận trong repository thông qua hệ thống quản lý của Git. Và ta có 2 dạng chính như sau.

- **Local Repository (Cục bộ):** Trên máy tính cá nhân, máy tính của chính các bạn làm việc.
- **Remote Repository (Từ xa):** Trên các nền tảng như GitHub, GitLab, Bitbucket,... phục vụ việc chia sẻ và cộng tác nhóm. Hay gọi cách khác là nơi làm việc của nhóm.

Repository đóng vai trò trung tâm trong quy trình làm việc, quyết định dự án của bạn có được quản lý bài bản hay không. Để hình dung rõ hơn, bạn có thể tưởng tượng: mọi đoạn code bạn viết ra đều được lưu trong Local Repository. Tuy nhiên, nếu máy tính bạn gặp sự cố như mất dữ liệu hoặc hỏng ổ cứng, bạn có thể mất toàn bộ mã nguồn nếu không có bản sao lưu nào.

Đó là lý do việc đẩy (push) mã nguồn lên Remote Repository trên GitHub là một giải pháp cần thiết. GitHub đóng vai trò như một “đám mây” dành riêng cho mã nguồn của bạn, còn Git chính là công cụ giúp bạn thực hiện việc đồng bộ hóa giữa local và remote: như push, pull, clone, fetch, v.v.

## 2.2 Các lệnh về Terminal
Trước khi tạo repository, mình muốn bạn thực hành các lệnh sau với Terminal, đây là đối với Windows. Còn về MacOS thì mình không rành nên không đề cập được, nếu được mình rất cảm ơn nếu bạn đóng góp thêm ý kiếm cũng như các câu lệnh ở Link sau: [Git-Report](https://github.com/DungLe939/git-report-hcmus.git)

Bạn sẽ làm quen với các lệnh và tổ hợp phím sau, bạn hãy xem qua và yên tâm mình sẽ hướng dẫn bạn thực hành những lệnh này ở phần sau.
- `Window + R + Enter`:  Mở CMD nhanh.
- `cd [path]`: Lệnh di chuyển đến mục trong cmd.
- `cd ..`: Quay lại đường dẫn.
- `dir`: Liệt kê các File trên Folder hiện tại.
- `mkdir [nameFolder]`: Tạo một Folder mới.
- `echo [Content] > [nameFile.định dạng]`: Tạo ra một File theo định dạng bạn tạo có nội dung là Content.
- `del [yourFile]`: Xóa File, lệnh del chỉ dành cho việc xóa File chứ không phải Folder.

Đây là những lệnh mình hay xài, dĩ nhiên bạn có thể sử dụng các thao tác bằng chuột để mở, tạo, lưu file. Nhưng trong này mình muốn các bạn hãy dùng bằng Terminal để có thể tập làm quen.

Nếu các bạn có gặp vấn đề gì về lỗi Terminal, phiền bạn hãy sử dụng Git Bash here. Git bash nó xem đảm bảo bạn có thể chắc chắn xài được các câu lệnh.

 **\*Cách sử dụng**: Nếu bạn đã cài Git bạn sẽ nhấn chuột phải vào khoảng trống Folder hiện tại của bạn nó sẽ có Git Bash để bạn có thể dử dụng.

---

## 2.3 Thực hành lệnh Terminal
Trong lần thực hành này tôi muốn các bạn làm quen với terminal nếu có vướng mắc hay cần thêm thông tin hãy hỏi AI để bạn biết thêm chi tiết hơn. Bài thực hành có yêu cầu như sau:

- Bước 1: Thực hiện mở `cmd` nhanh bằng phím tắt `Window + R + Enter`.
- Bước 2: Làm quen với thao tác di chuyển `cd` và `cd..` để di chuyển vào nơi bạn muốn tạo Folder. 
- Bước 3: Tạo một Folder với tên là `Git-Test` bằng lệnh `mkdir`.
	- Di chuyển vào Folder `Git-Test`.
	- Tạo một file text (.txt) có tên là `chapter1.txt` bằng lệnh `echo`
	- Tạo file tên là `chapter2.txt`.
	- Check xem trong Folder đó có gì bằng lệnh `dir`.
	- Xóa file `chapter2.txt`.
- Bước 4: Mở Folder đó qua visual studio code bằng lệnh `code .`(code chấm).
