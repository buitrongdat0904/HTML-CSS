
## Cấu trúc thẻ danh sách có thứ tự và không có thứ tự

Cấu trúc thể hiện thẻ danh sách có thứ tự và không có thứ tự là tương tự nhau.

Cấu trúc phải theo các nguyên tắc sau đây:

- Lúc nào cũng phải tồn tại 1 cặp thẻ, không thể thiếu một trong 2:

    + Đối với danh sách có thứ tự, phải tồn tại cặp thẻ: < ol>< /ol>, < li>< /li>.
    + Đối với danh sách không có thứ tự, phải tồn tại cặp thẻ: < ul>< /ul>, < li>< /li>.

- Bên trong thẻ < ol>< /ol> (hoặc < ul>< /ul>) chỉ chứa trực tiếp một thẻ duy nhất < li>< /li>.
- Bên trong thẻ < li>< /li> chứa được hầu hết các thẻ HTML/HTML5, tuy nhiên không được chứa 
  một số thẻ sau đây: < html>< /html>, < meta>< /meta>, < body>< /body>, < title>< /title>, < link>< /link>.
   Và một số thẻ không nên chứa như: < style>< /style>, < script>< /script>.
   
        <ol>
        <li></li>
        <li></li>
        </ol>

        <ul>
        <li></li>
        <li></li>
        </ul>
  

  # Thẻ <nav>
  ## Định nghĩa và sử dụng
- Tag <nav> định nghĩa liên kết điều hướng (navigation).
- Tag <nav> thường sử dụng cho global menu, local link, topic path, pager link,...
- Nội dung bên trong <nav> thường là một danh sách <ul> hoặc <ol>.
### Cấu trúc

    <nav>
        <ul>
            <li><a href="#">Trang chủ<a></li>
            <li><a href="#">Giới thiệu<a></li>
            <li><a href="#">Sản phẩm<a></li>
            <li><a href="#">Liên hệ<a></li>
        </ul>
    </nav>


  # Thẻ <header>

## Định nghĩa và sử dụng
- Tag <header> định nghĩa khu vực header (phần đầu) của trang.
- Thường được dùng cho phần giới thiệu hay chứa các thành phần chuyển hướng (navigation).
### Cấu trúc

    <header></header>
 ### Ví dụ 
    <header>
          HEADER

          <nav>
              <ul>
                  <li><a href="#">Trang chủ<a></li>
                  <li><a href="#">Giới thiệu<a></li>
                  <li><a href="#">Sản phẩm<a></li>
                  <li><a href="#">Liên hệ<a></li>
              </ul>
          </nav>
      </header>


# section

## Định nghĩa và sử dụng
- Tag < section> định nghĩa một khu vực (vùng bao) trong văn bản HTML.
- Tag < section> bên trong thường chứa một < hx> và nội dung.

## Cấu trúc

    <section>
    <h2>Tiêu đề section</h2>
    ...
    </section>

### Ví dụ
    <section id="layout">
        <header>
            HEADER

            <nav>
                <ul>
                    <li><a href="#">Trang chủ<a></li>
                    <li><a href="#">Giới thiệu<a></li>
                    <li><a href="#">Sản phẩm<a></li>
                    <li><a href="#">Liên hệ<a></li>
                </ul>
            </nav>
        </header>
    </section>


# footer
## Định nghĩa và sử dụng
- Tag < footer> định nghĩa khu vực footer (phần cuối) của trang.
- Thường chứa các thông tin liên lạc của tác giả, nguồn gốc của bài viết.
## Cấu trúc
 
    <footer></footer>

# Những thẻ thuộc nhóm inline


- Những thẻ thuộc nhóm inline là những thẻ cơ bản của HTML/XHTML, chỉ được dùng để chứa nội dung cho text hoặc các thẻ inline khác.
- - Bản thân text cũng có thể coi thuộc nhóm inline.
- Những thẻ thuộc nhóm inline nên được bao ngoài bởi nhóm các thẻ block, vì các thẻ block sẽ lo nhiệm vụ dàn trang web, còn 
  các thẻ thuộc nhóm inline chỉ để hiển thị nội dung cho văn bản.
- Những thẻ thuộc nhóm inline có thể được lồng vào nhau.
- Không được sử dụng các thẻ khác bên trong các thẻ inline, cách sử dụng sau đây là không đúng chuẩn:

## Thẻ liên kết <a></a>
 - Thẻ liên kết < a>< /a> dùng để tạo một liên kết từ trang web này sang trang web khác, từ vị trí này sang vị trí khác hay
   dùng để mở ra một object nào đó (có thể là file words, excel, pdf, mp3, movie,...), thẻ này có một thuộc tính bắt buộc:

    - href: Chứa đường dẫn cụ thể tới mục tiêu liên kết.

## Thẻ hiển thị một image < img/>
- Thẻ hiển thị một image < img/> dùng để nhúng một ảnh thông qua thuộc tính src, thẻ này có 2 thuộc tính bắt buộc:

    + src: Chứa đường dẫn tham chiếu tới image.
    + alt: Được sử dụng như một văn bản thay thế khi image không hiển thị (hoặc không có sẵn).
- Cấu trúc của thẻ < img/> không có sử dụng thẻ đóng (không dùng <img></img>), mà sử dụng ký tự kết thúc là một khoảng t
    rắng và ký tự "/".

## Thẻ ngắt đoạn văn bản < br/>
- Thẻ ngắt đoạn văn bản < br/> dùng để xuống dòng văn bản trong cùng một đoạn văn.
- Cấu trúc của thẻ <br /> không có sử dụng thẻ đóng (không dùng < br>< /br>), mà sử dụng 
    ký tự kết thúc là một khoảng trắng và ký tự "/".


## Thẻ nhóm các inline < span>< /span>
- Thẻ nhóm các inline < span>< /span> dùng để nhóm một hay nhiều thẻ inline khác nhau, thẻ này không có ý nghĩa về mặt hiển thị, 
    chỉ hỗ trợ định dạng các inline thông qua CSS hoặc Javascript.

## Thẻ hiển thị hình ảnh mạnh < strong></strong>
- Thẻ hiển thị hình ảnh mạnh < strong>< /strong> mục đích đánh dấu văn bản, văn bản được đánh dấu sẽ hiển thị dạng in đậm.
- Tham khảo thêm về thẻ < strong>< /strong>.

## Thẻ dùng để nhấn mạnh nội dung văn bản < em>< /em>
- Thẻ dùng để nhấn mạnh nội dung văn bản <em></em> mục đích nhấn mạnh văn bản nhằm gây chú ý cho người xem, văn bản được đánh dấu
   sẽ hiển thị bằng hình dạng, in nghiên, màu sắc.

NGOÀI RA CÒN RẤT NHIỀU THẺ INLINE KHÁC