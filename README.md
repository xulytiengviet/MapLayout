# MapLayout Studio

Trình biên tập bố cục bản đồ trên trình duyệt do **Long Ngo** thiết kế. Giấy phép **MIT (2026)**.

## Chức năng
- MapLibre GL JS với 11 kiểu bản đồ nền raster, tìm kiếm Nominatim, tọa độ.
- Nhập GeoJSON, KML, KMZ, GPX, Shapefile ZIP; tự tạo lớp bản đồ và chú giải.
- A4/A3, trang SVG đơn vị mm, hai khung bản đồ phụ dạng ảnh minh họa, lưới kinh/vĩ độ DMS/thập phân, thanh tỷ lệ ước tính, hướng Bắc, nhãn tác giả, ngày.
- Kéo thành phần SVG, vẽ hình, ghi chú, thêm logo, xuất PNG/PDF/SVG và JSON dự án.

## Triển khai
Website tĩnh: bật GitHub Pages cho nhánh `main`, thư mục `/ (root)`. Không cần Node hoặc backend.

## Hạn chế đã biết
Bản đồ phụ hiện sử dụng ảnh cùng khung nhìn chính; chưa có tính toán thực sự phạm vi quốc gia/vùng. Hình ảnh nền được nhúng dạng raster trong SVG, không phải vector hoàn toàn. PDF sử dụng ảnh PNG trang nên chưa bảo đảm font được nhúng hoặc bản đồ vector. Thước tỷ lệ là gần đúng theo vĩ độ và kinh độ; không sử dụng để đo đạc trắc địa. UTM mới là tùy chọn nhãn, chưa thực hiện chuyển đổi UTM. Một số nhà cung cấp raster có thể chặn xuất canvas (CORS). Tìm địa danh dùng dịch vụ Nominatim công khai có giới hạn sử dụng; dữ liệu không tự tải lên máy chủ ứng dụng. CRX của bên thứ ba chỉ dùng tham khảo chức năng, không tái sử dụng mã nguồn sở hữu của họ.
