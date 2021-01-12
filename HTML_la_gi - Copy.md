# HTML là gì ?
1. HTML là viết tắt của Hyper Text Markup Language
2. HTML là ngôn ngữ đánh dấu tiêu chuẩn để tạo các trang Web
3. HTML mô tả cấu trúc của một trang Web
4. HTML bao gồm một loạt các phần tử
5. Các phần tử HTML cho trình duyệt biết cách hiển thị nội dung
6. Các phần tử HTML gắn nhãn các phần nội dung như "đây là một tiêu đề", "đây là một đoạn văn", "đây là một liên kết", v.v.

#### Một tài liệu HTML đơn giản

    <h1>Tiêu đề 01</h1>

    <ul>
    <li><a href="#">Link 01</a></li>
    <li><a href="#">Link 02</a></li>
    <li><a href="#">Link 03</a></li>
    <li><a href="#">Link 04</a></li>
    <li><a href="#">Link 05</a></li>
    </ul>

    <div>Nội dung chính</div>

    <div>Nội dung phụ</div>

    <div>
    <p>Tên công ty</p>
    <p>Địa chỉ</p>
    </div>
# Các thẻ trong HTML - Tag trong HTML

Như đã trình bày ở trên, HTML là ngôn ngữ đánh dấu bằng thẻ (tag) và sử dụng các thẻ khác nhau để định dạng nội dung. Những thẻ này được chứa trong hai dấu ngoặc đơn < tên thẻ>. Trừ một vài thẻ, hầu hết các thẻ đều có các thẻ đóng tương ứng với nó. Ví dụ, thẻ < html> có thẻ đóng tương ứng là < /html> và thẻ < body> có thẻ đóng tương ứng là < /body> ...

#### Ví dụ trên về tài liệu HTML đã sử dụng các thẻ sau đây:

|Tag          | Miêu tả                                                                                     | 
|:------------|:--------------------------------------------------------------------------------------------|
|<!DOCTYPE...>| Còn gọi là thẻ khai báo một tài liệu HTML. Thẻ này xác định loại tài liệu và phiên bản HTML.|
|< head>      |Thẻ này đại diện cho đầu trang tài liệu mà có thể giữ các thẻ HTML như < title>, < link> ... | 
|< title>	  |Thẻ < title> được sử dụng trong thẻ < head> chỉ tiêu đề tài liệu.                            | 
|< body>	  |Thẻ này đại diện cho thân tài liệu và giữ các thẻ như < h1>, < div>, < p> ...                |
|< h1>	      | Thẻ này đại diện cho các tiêu đề trang.                                                     |
|< p>         |Thẻ này đại diện cho đoạn văn.                                                               |

# Các thẻ HTML cơ bản (HTML Tag)

## Nhóm các thẻ block

Nhóm các thẻ block: là các thẻ dùng để sắp xếp bố cục cho trang web.

- Thẻ định dạng tiêu đề < hx>
  Gồm các thẻ từ < h1> cho đến < h6>, được sử dụng để định nghĩa tiêu đề cho nội dung HTML, giúp cho trình duyệt nhận biết được tiêu đề của một nội dung.

- Thẻ định dạng đoạn văn bản < p>
  Giúp trình duyệt xác định được đoạn văn bản trong trang HTML, thẻ này chỉ có thể chứa các thẻ thuộc nhóm inline, gồm: text, image, link, button,....

- Thẻ phân chia khu vực < div>
  Ta có thể hiểu đây là sự phân chia khu vực hay vùng, sự phân chia này sẽ giúp cho trình duyệt hiểu rõ những vùng được bố cục trên trang web..

- Thẻ xác định danh sách < dl>, < dt>, < dd>
  Sử dụng cho danh sách có các mục và có nội dung mô tả cho các mục.

- Thẻ danh sách có thứ tự < ol>, < li>
  Được sử dụng cho danh sách có thứ tự.

- Thẻ danh sách không có thứ tự < ul>, < li>
  Được sử dụng cho danh sách không có thứ tự.

- Thẻ xác định menu link điều hướng (navigation) < nav>
  Chứa các liên kết giữa các trang với nhau.

- Thẻ xác định phần đầu trang web < header>
  Chứa tất cả phần đầu của trang web, gồm: logo, dòng mô tả, liên kết, ...

- Thẻ xác định khu vực có nội dung < section>
  Bao ngoài các nội dung lớn thường có chưa tiêu đề.

- Thẻ xác định một bài viết, một nội dung riêng biệt < article>
  Nội dung gồm các tin tức chi tiết, bài báo, ...

- Thẻ xác định nội dung phụ bên cạnh nội dung chính (phần sidebar) < aside>
  Tất cả phần sidebar chứa liên kết, banner, ...

- Thẻ xác định phần nội dung cuối trang web < footer>
  Chứa tất cả phần cuối của trang web, gồm: liên kết phụ, logo, copyright, thông tin liên hệ, ...

- Thẻ xác định hình ảnh có chú thích < figure> - < figcaption>
  Giải thích rõ nghĩa hơn cho image.

## Thẻ định dạng tiêu đề

### Định nghĩa và cách dùng

- Thẻ < hx>: chữ "h" viết tắc của từ "headings" nghĩa là đề mục, hoặc tiêu đề.
- Thẻ < hx> : Sử dụng để định nghĩa tiêu đề cho nội dung HTML, giúp cho trình duyệt nhận biết được tiêu đề của một nội dung.
- Thẻ < hx> có giá trị từ < h1> tới < h6>, trong đó mức độ quan trọng giảm từ < h1> tới < h6> (hay ta có thể hiểu:
 tiêu đề lớn nhất là < h1>, và tiêu đề nhỏ nhất là < h6>).
- Nội dung bên trong < hx>< /hx> chỉ nên chứa các thẻ thuộc nhóm inline.
- Thẻ < hx>< /hx> chỉ nên thể hiện tiêu đề, không dùng cho mục đích khác.

Html viết:

    <!DOCTYPE html>
    <html>
    <head>
    <meta charset=utf-8" />
    <title>Tiêu đề trang web</title>
    </head>

    <body>
    <h1>Đây là tiêu đề quan trọng nhất (lớn nhất)</h1>
    <h2>Đây là tiêu đề quan trọng thứ nhì (lớn thứ nhì)</h2>
    <h3>Đây là tiêu đề quan trọng thứ ba (lớn thứ ba)</h3>
    <h4>Đây là tiêu đề quan trọng thứ tư (lớn thứ tư)</h4>
    <h5>Đây là tiêu đề quan trọng thứ năm (lớn thứ năm)</h5>
    <h6>Đây là tiêu đề ít quan trọng nhất (nhỏ nhất)</h6>
    </body>
    </html>

Hiển thị trình duyệt:

# Đây là tiêu đề quan trọng nhất (lớn nhất)
## Đây là tiêu đề quan trọng thứ nhì (lớn thứ nhì)
### Đây là tiêu đề quan trọng thứ ba (lớn thứ ba)
#### Đây là tiêu đề quan trọng thứ tư (lớn thứ tư)
##### Đây là tiêu đề quan trọng thứ năm (lớn thứ năm)
###### Đây là tiêu đề ít quan trọng nhất (nhỏ nhất)

Thẻ < h1> là thẻ quan trọng nhất trong trang HTML, trong một trang html thường người ta sử dụng < h1> một lần duy nhất cho logo, hoặc dòng mô tả trang web (mục đích SEO), mục đích của < h1> là khai báo cho trình duyệt biết đâu là phần quan trọng nhất của trang web.

HTML viết

    <!DOCTYPE html>
    <html>
    <head>
    <meta charset=utf-8" />
    <title>Tiêu đề trang web</title>
    </head>

    <body>
    <h1>Logo</h1>
    <h2>Tiêu đề lớn</h2>
    <p>Nội dung của tiêu đề lớn</p>

    <h3>Tiêu đề nhỏ</h3>
    <p>Nội dung của tiêu đề nhỏ</p>
    </body>
    </html>

Hiển thị trình duyệt:
# Logo
## Tiêu đề lớn
Nội dung của tiêu đề lớn

### Tiêu đề nhỏ
Nội dung của tiêu đề nhỏ

## Thẻ định dạng đoạn văn bản

- Thẻ < p>< /p> viết tắt của từ "paragraphs" có nghĩa là đoạn văn.
- Thẻ <p></p> giúp trình duyệt xác định được đoạn văn bản trong trang HTML, thẻ này chỉ có thể chứa các thẻ 
  thuộc nhóm inline, gồm: text, image, link, button,...

#### HTML viết

    <!DOCTYPE html>
    <html>
    <head>
    <meta charset=utf-8" />
    <title>Tiêu đề trang web</title>
    </head>

    <body>
    <p>Đây là đoạn văn</p>
    </body>
    </html>

#### Hiển thị trình duyệt:

  <!DOCTYPE html>
    <html>
    <head>
    <meta charset=utf-8" />
    <title>Tiêu đề trang web</title>
    </head>
    <body>
    <p>Đây là đoạn văn</p>
    </body>
    </html>

    Để ngắt đoạn cho đoạn văn ta có thể dùng 2 cách:

### Ngắt đoạn cùng dòng: sử dụng thẻ < br/> (< br/> là thẻ thuộc nhóm inline).

#### HTML viết

    <!DOCTYPE html>
    <html>
    <head>
    <meta charset=utf-8" />
    <title>Tiêu đề trang web</title>
    </head>

    <body>
    <p>Đây là đoạn văn dài rất dài rất dài rất dài<br />
    rất dài rất dài rất dài rất dài.</p>
    </body>
    </html>

#### Hiển thị trình duyệt:

<!DOCTYPE html>
<html>
<head>
<meta charset=utf-8" />
<title>Tiêu đề trang web</title>
</head>

<body>
<p>Đây là đoạn văn dài rất dài rất dài rất dài<br />
rất dài rất dài rất dài rất dài.</p>
</body>
</html>

- Ngắt đoạn khác dòng: sử dụng 2 thẻ <p></p> để ngắt đoạn khác dòng, tránh trường hợp sử dụng 2 lần thẻ < br/> vì về mặt ý nghĩa 
  của thẻ sẽ không còn chính xác, điều này sẽ gây khó khăn cho trình duyệt phân biệt đâu là cùng đoạn, đâu là khác đoạn.

#### HTML viết
    <!DOCTYPE html>
    <html>
    <head>
    <meta charset=utf-8" />
    <title>Tiêu đề trang web</title>
    </head>

    <body>
    <p>Đây là đoạn văn thứ nhất.</p>
    <p>Đây là đoạn văn thứ hai.</p>
    </body>
    </html>

Hiển thị trình duyệt:
    <!DOCTYPE html>
    <html>
    <head>
    <meta charset=utf-8" />
    <title>Tiêu đề trang web</title>
    </head>
    <body>
    <p>Đây là đoạn văn thứ nhất.</p>
    <p>Đây là đoạn văn thứ hai.</p>
    </body>
    </html>













