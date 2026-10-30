# Bài 2 : Quản lý Quyền truy cập Báo cáo Tài chính

## Phần 1 : Bản thiết kế phân quyền

   1. Viewer : chỉ dành cho những người chỉ có thể đọc và không thể làm gì khác , phù hợp với cho nhân viên xem
    
   2. commenter : phù hợp với những người mình muốn chia sẽ để lấy nhận xét và người đó chỉ có thể đọc, viết bình luận không thể viết hay làm gì file

   3. Editor : quyền này cho phép người khác có thể chỉnh sửa , viết , và làm mọi thứ về file ,phù hợp để chia sẽ dữ liệu cho cấp trên

## Phần 2 :  Quy trình 3 bước xử lý khi phát hiện dữ liệu bị chia sẻ sai quyền.

  - Bước 1 : Đổi ngay link chia sẽ chung sang link chia sẽ hạn chế
  - Bước 2 : Xóa hẳn email ứng viên khỏi danh sách chia sẽ
  - Bước 3 : Tắt quyền chia sẽ link của editor

** Bẫy dữ liệu : ** Khi muốn biết người lạ đã copy , hay chụp màn hình dữ liệu hay chưa
 * Vào mục Drive log events, lọc theo:

        1. Document ID của file danh sách ứng viên.
        
        2. Actor / Email: Địa chỉ của ứng viên (hoặc lọc sự kiện Anonymous nếu link để Public).
        
        3. Event: Tìm các hành vi Download, Print, Copy, View, Edit.
        
         
