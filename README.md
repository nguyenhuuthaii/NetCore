//cấu trúc Project .NET MVC
MVCMOVIE : Tên Project
Controllers: Thư mục chứa các Controller (Code để xử lý yêu cầu từ View gửi về)
ModelS: Chứa các  lớp chứa CSDL của ứng dụng
Views: Thư mục chứa các thành phần hiển thị giao diện người dùng
wwwroot: Thư mục chứa các FILE của dự án(HTML,CSS,JS)
appsettings.json và Program.cs : file chứa code cấu hình dự án
 
//router. NET MVC
mvc sẽ là bộ điều khiển(Controller) và các hành động  bên trong (Action) thông qua URL
Logic định tuyến MVC sử dụng dạng: /[Controller]/[Action]/[Pramenters]
Định tuyến đc cấu hình trong file Program.cs:
     app.MapControllerRouter(
        name:"default",
        pattern:"{controller=Home}/{action=Index}/{id?}");

//Controller.NET MVC
Tên của Controller bắt buộc phải có hậu tố Controller VD:
   StudentController,PersonController
Nằm trong thư mục Controller
Nhiệm vụ của Controller:
 -Xử lý các yêu cầu của người dùng gửi tới View.
 -Truy xuất dữ liệu trong cơ sở dữ liệu.
 -Gọi các mẫu View và trả vể dữ liệu.

 //View.NET MVC
 Có phần mở rộng là ".cshtml"
 Nằm trong thư mục Views/Controller_Name(tương ứng với HelloWorldController sẽ có  thư mục HelloWorld trong thư mục Views)
 Nhiệm vụ của View: cung cấp giao diện người dùng (HTML) bằng C#