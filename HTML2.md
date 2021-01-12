# Các thẻ danh sách có thứ tự và không có thứ tự

## Danh sách có thứ tự và không có thứ tự

Định nghĩa danh sách trong HTML/HTML5 có nhiều dạng khác nhau, mỗi dạng sẽ theo một cấu trúc thẻ khác nhau, do đó việc hiểu rõ 
danh sách rất quan trọng, nếu bạn chưa nắm rõ cách định nghĩa về danh sách thì bạn không thể hiểu hết được bài học này, xin hãy xem trước định nghĩa về danh sách trong HTML/HTML5.

## Danh sách có thứ tự

Để thể hiện danh sách có thứ tự ta sử dụng cặp thẻ: < ol>< /ol> và < li>< /li>, trong đó:

< ol>< /ol> là viết tắt của chữ "ordered list" có nghĩa là danh sách có thứ tự.
< li>< /li> viết tắt của chữ "list item" có nghĩa là mục của danh sách.
Danh sách sau đây gọi là danh sách có thứ tự:

    1. Cá lóc kho tiêu
    2. Cá rô kho tộ
    3. Cá thu chiên xoài bằm
    4. Cá điêu hồng nấu ngót

Hoặc:

    a) Học HTML
    b) Học XHTML
    c) Học HTML5
    d) Học CSS2
    e) Học CSS3

### HTML viết

    <!DOCTYPE html>
    <html>
    <head>
    <meta charset=utf-8" />
    <title>Tiêu đề trang web</title>
    </head>

    <body>
    <ol>
    <li>Cá lóc kho tiêu</li>
    <li>Cá rô kho tộ</li>
    <li>Cá thu chiên xoài bằm</li>
    <li>Cá điêu hồng nấu ngót</li>
    </ol>
    </body>
    </html>

### Hiển thị trình duyệt:

1. Cá lóc kho tiêu
2. Cá rô kho tộ
3. Cá thu chiên xoài bằm
4. Cá điêu hồng nấu ngót

Số thứ tự của danh sách trình duyệt sẽ tự thêm vào.

## Danh sách không có thứ tự
Để thể hiện danh sách không có thứ tự ta sử dụng cặp thẻ: < ul>< /ul> và < li>< /li>, trong đó:
< ul>< /ul> là viết tắt của chữ: unordered list có nghĩa là danh sách không có thứ tự
< li>< /li> viết tắt của chữ: list item có nghĩa là mục của danh sách.
Danh sách sau đây gọi là danh sách không có thứ tự:

      Trang chủ
      Giới thiệu
      Sản phẩm
      Dịch vụ
      Liên hệ

      Hoặc:

      Học HTML
      Học XHTML
      Học HTML5
      Học CSS2
      Học CSS3

### HTML viết
    <!DOCTYPE html>
    <html>
    <head>
    <meta charset=utf-8" />
    <title>Tiêu đề trang web</title>
    </head>

    <body>
    <ul>
    <li>Trang chủ</li>
    <li>Giới thiệu</li>
    <li>Sản phẩm</li>
    <li>Dịch vụ</li>
    <li>Liên hệ</li>
    </ul>
    </body>
    </html>

Hiển thị trình duyệt:

  <ul>
  <li>Trang chủ</li>
  <li>Giới thiệu</li>
  <li>Sản phẩm</li>
  <li>Dịch vụ</li>
  <li>Liên hệ</li>
  </ul>

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

