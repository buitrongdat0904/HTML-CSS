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

## Các thẻ hiển thị đầu đề (heading) trong HTML

    <!DOCTYPE html>
    <html>
    <head>
    <title>Day la tieu de - Vi du dau de</title>
    </head>
    <body>
    <h1>Day la dau de 1</h1>
    <h2>Day la dau de 2</h2>
    <h3>Day la dau de 3</h3>
    <h4>Day la dau de 4</h4>
    <h5>Day la dau de 5</h5>
    <h6>Day la dau de 6</h6>
    </body>
    </html>

![tieude](https://vietjack.com/html/images/vi-du-html-1.PNG)

# Phần tử HTML
Phần tử HTML được xác định bởi thẻ bắt đầu, một số nội dung và thẻ kết thúc.

## Phần tử HTML
Phần tử HTML là tất cả mọi thứ từ thẻ bắt đầu đến thẻ kết thúc:
< tagname > Nội dung ở đây ... < / tagname >
Ví dụ về một số phần tử HTML:
    < h1 > Tiêu đề đầu tiên của tôi < / h1 >
    < p > Đoạn đầu tiên của tôi. < / p >

    Lưu ý: Một số phần tử HTML không có nội dung (như phần tử <br>).
     Các phần tử này được gọi là phần tử rỗng. Các phần tử trống không có thẻ kết thúc!

## Các phần tử HTML lồng nhau
** Ta có ví dụ: ** 

    <!DOCTYPE html>
    <html>
    <body>

    <h1>My First Heading</h1>
    <p>My first paragraph.</p>

    </body>
    </html>

** Giải thích ví dụ:**

    Phần <html>tử là phần tử gốc và nó định nghĩa toàn bộ tài liệu HTML.
    Nó có một thẻ bắt đầu <html>và một thẻ kết thúc </html>.
    Sau đó, bên trong <html>phần tử có một <body> phần tử:
    
        <h1>My First Heading</h1>
        <p>My first paragraph.</p>








