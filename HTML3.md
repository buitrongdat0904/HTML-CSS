# Thẻ phân chia khu vực

## Định nghĩa và cách dùng thẻ < div>

- Thẻ < div>< /div> viết tắt của từ "division" có nghĩa là phân chia, ta có thể hiểu đây là sự phân chia khu vực hay vùng,
  sự phân chia này sẽ giúp cho trình duyệt hiểu rõ những vùng được bố cục trên trang web.
- Có thể chứa hầu hết các thẻ trong HTML/XHTML.
- Một số thẻ không được chứa bên trong < div>< /div>: < html>< /html>, < meta>< /meta>, < body>< /body>,
  < title>< /title>, < link>< /link>.
- Một số thẻ không nên chứa bên trong < div>< /div>: < style>< /style>, < script>< /script>.
- Một số khu vực khuyên sử dụng thẻ < div>< /div>:

    - Header, global navigation, page body, content, sidebar, footer (Xem lại cấu trúc cơ bản của trang web)
    - Một số khu vực lớn, cấu trúc có nhiều thẻ bên trong thì cũng nên nhóm lại bằng thẻ < div>< /div> để tiện cho việc điều khiển.

Xem ví dụ để hiểu rõ hơn về thẻ < div>< /div>, đoạn code bên dưới có sử dụng thuộc tính id, chúng ta có thể xem ở phần tham khảo thuộc tính id.

### HTML viết

    <!DOCTYPE html>
    <html>
    <head>
    <meta charset=utf-8" />
    <title>Tiêu đề trang web</title>
    </head>

    <body>
    <div id="header">Viết nội dung phần header ở đây</div>

    <div id="gNav">Viết nội dung phần global navigation ở đây</div>

    <div id="pageBody">
    <div id="content">Viết nội dung phần content ở đây</div>
    <div id="sidebar">Viết nội dung phần sidebar ở đây</div>
    </div>

    <div id="footer">Viết nội dung phần footer ở đây</div>
    </body>
    </html>

### Hiển thị trình duyệt:

<div id="header">Viết nội dung phần header ở đây</div>
<div id="gNav">Viết nội dung phần global navigation ở đây</div>
<div id="pageBody">
<div id="content">Viết nội dung phần content ở đây</div>
<div id="sidebar">Viết nội dung phần sidebar ở đây</div>
<div id="footer">Viết nội dung phần footer ở đây</div>

# Thẻ xác định danh sách

## Định nghĩa
Định nghĩa danh sách trong HTML/HTML5 có nhiều dạng khác nhau, mỗi dạng sẽ theo một cấu trúc thẻ khác nhau, do đó việc hiểu rõ danh sách rất quan trọng, nếu bạn chưa nắm rõ cách định nghĩa về danh sách thì bạn không thể hiểu hết được bài học này, xin hãy xem trước định nghĩa về danh sách trong HTML/HTML5.

Thẻ xác định danh sách (có đề mục và mô tả đề mục) là một bộ gồm 3 thẻ:

- < dl>< /dl> viết tắt của chữ "definition list" có nghĩa là sự xác định (hay định nghĩa) danh sách.
- < dt>< /dt> viết tắt của chữ "defines an item" có nghĩa là xác định (hay định nghĩa) một mục.
- < dd>< /dd> viết tắt của chữ "defines describe an item" có nghĩa là xác định (hay định nghĩa) một mô tả của một mục.

Thẻ xác định danh sách sử dụng cho danh sách có các mục và có nội dung mô tả cho các mục, không sử dụng cho danh sách không có phần nội dung mô tả.

### HTML viết

    <!DOCTYPE html>
    <html>
    <head>
    <meta charset=utf-8" />
    <title>Tiêu đề trang web</title>
    </head>

    <body>
    <dl>
    <dt>Trái cây:</dt>
    <dd>giúp bỗ sung vitamin cho cơ thể.</dd>

    <dt>Nước:</dt>
    <dd>giúp chúng ta tăng cường lượng nước cần cho cơ thể.</dd>

    <dt>Thịt:</dt>
    <dd>giúp cơ thể tăng cường đạm, và chất béo.</dd>
    </dl>
    </body>
    </html>

### Hiển thị trình duyệt:
  <dl>
    <dt>Trái cây:</dt>
    <dd>giúp bỗ sung vitamin cho cơ thể.</dd>
    <dt>Nước:</dt>
    <dd>giúp chúng ta tăng cường lượng nước cần cho cơ thể.</dd>
    <dt>Thịt:</dt>
    <dd>giúp cơ thể tăng cường đạm, và chất béo.</dd>
    </dl>
  

## Cấu trúc và cách dùng
Cấu trúc thẻ xác định danh sách phải theo các nguyên tắc sau đây:

- Lúc nào cũng phải tồn tại 3 thẻ, không thể thiếu một trong 3: < dl>< /dl>, < dt>< /dt>, < dd>< /dd>.
- Bên trong thẻ < dt>< /dt> chỉ chứa được các thẻ thuộc nhóm inline.
- Bên trong thẻ < dd>< /dd> chứa được hầu hết các thẻ HTML/HTML5, tuy nhiên không được chứa một số thẻ sau đây:
 < html>< /html>, < meta>< /meta>, < body>< /body>, < title>< /title>, < link>< /link>. Và một số thẻ không nên chứa như:
  < style>< /style>, < script>< /script>.
- Thẻ < dt>< /dt> và < dd>< /dd> phải được viết trực tiếp bên trong < dl>< /dl>:

        <dl>
        <dt></dt>
        <dd></dd>

        <dt></dt>
        <dd></dd>
        </dl>

 
Bên trong thẻ <dl></dl> chỉ chứa trực tiếp thẻ < dt>< /dt> và < dd>< /dd>, không được xen kẻ bất kỳ thẻ nào khác, những cấu trúc như bên dưới đây là sai, không đúng chuẩn W3C:

    <dl>
    <h2></h2>
    <dt></dt>
    <dd></dd>
    </dl>

    <dl>
    <dt></dt>
    <p></p>
    <dd></dd>
    </dl>

    <dl>
    <dt></dt>
    <div>
    <dd></dd>
    </div>
    </dl>

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
