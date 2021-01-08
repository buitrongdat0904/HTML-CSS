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
**Ta có ví dụ:** 

    <!DOCTYPE html>
    <html>
    <body>

    <h1>My First Heading</h1>
    <p>My first paragraph.</p>

    </body>
    </html>

**Giải thích ví dụ:**

Phần tử **< html>**là phần tử gốc và nó định nghĩa toàn bộ tài liệu HTML.
Nó có một thẻ bắt đầu < html>và một thẻ kết thúc < /html>.
Sau đó, bên trong < html>phần tử có một < body> phần tử:

        <h1>My First Heading</h1>
        <p>My first paragraph.</p>

Phần **< body>**tử xác định phần thân của tài liệu.

Nó có một thẻ bắt đầu < body>và một thẻ kết thúc < /body>.

Sau đó, bên trong < body>phần tử có hai phần tử khác: < h1>và < p>:

    <h1>My First Heading</h1>
    <p>My first paragraph.</p>

Phần **< h1>**tử xác định một tiêu đề.

Nó có thẻ bắt đầu < h1>và thẻ kết thúc < /h1>:

    <h1>My First Heading</h1>

Phần **< p>**tử xác định một đoạn văn.

Nó có thẻ bắt đầu < p>và thẻ kết thúc < /p>:

    <p>My first paragraph.</p>

## Không bao giờ bỏ qua thẻ kết thúc
Một số phần tử HTML sẽ hiển thị chính xác, ngay cả khi bạn quên thẻ kết thúc:

Thí dụ:

    <html>
    <body>

    <p>This is a paragraph
    <p>This is a paragraph

    </body>
    </html>

Tuy nhiên, đừng bao giờ dựa vào điều này! Kết quả không mong muốn và có thể xảy ra lỗi nếu bạn quên thẻ kết thúc!

### Phần tử HTML trống

Phần tử HTML không có nội dung được gọi là phần tử trống.

Các **<br>**thẻ định nghĩa một ngắt dòng, và là một yếu tố có sản phẩm nào mà không có một thẻ đóng:

Thí dụ:

    <p>This is a <br> paragraph with a line break.</p>

## HTML không phân biệt chữ hoa chữ thường

Các thẻ HTML không phân biệt chữ hoa chữ thường: 

    <P>có nghĩa là giống như <p>.

# Thuộc tính HTML
Thuộc tính HTML cung cấp thông tin bổ sung về các phần tử HTML.

## Thuộc tính HTML
1. Tất cả các phần tử HTML có thể có các thuộc tính
2. Các thuộc tính cung cấp thông tin bổ sung về các phần tử
3. Các thuộc tính luôn được chỉ định trong thẻ bắt đầu
4. Các thuộc tính thường có trong các cặp tên / giá trị như: name = "value"

## Thuộc tính href
Các **<a>** thẻ định nghĩa một siêu liên kết. 
Các hrefthuộc tính xác định URL của trang liên kết đi vào:

Thí dụ:

    <a href="https://www.w3schools.com">Visit W3Schools</a>

Bạn sẽ tìm hiểu thêm về các liên kết trong chương Liên kết HTML của chúng tôi .

## Thuộc tính src
Các **< img>**thẻ được sử dụng để nhúng một hình ảnh trong một trang HTML. 
Các srcquy định cụ thể thuộc tính đường dẫn đến hình ảnh sẽ được hiển thị:
Thí dụ:

    <img src="img_girl.jpg">

Có hai cách để chỉ định URL trong src thuộc tính:

1. URL tuyệt đối - Liên kết đến một hình ảnh bên ngoài được lưu trữ trên một trang web khác.
    Ví dụ: 

        src = "https://www.w3schools.com/images/img_girl.jpg".


2. URL tương đối 
    - Liên kết đến một hình ảnh được lưu trữ trong trang web. Ở đây, URL không bao gồm tên miền. Nếu URL bắt đầu mà không có dấu gạch chéo, nó sẽ liên quan đến trang hiện tại.
     Ví dụ: 
            src = "img_girl.jpg".
    Nếu URL bắt đầu bằng dấu gạch chéo, nó sẽ có liên quan đến miền. 

        Ví dụ:
             src = "/ images / img_girl.jpg".
## Đường kẻ phân cách nằm ngang
Tag ** < hr/>** tạo một đường nằm ngang, bên trong trang HTML.
Tag < hr/> có thể được sử dụng để tách nội dung bên trong trang HTML.
## Ngắt dòng HTML
Phần **< br>**tử HTML xác định ngắt dòng.
Sử dụng < br>nếu bạn muốn ngắt dòng (một dòng mới) mà không bắt đầu một đoạn văn mới:

## Giải pháp - Phần tử <pre> HTML
Phần **< pre>**tử HTML xác định văn bản được định dạng trước.

Văn bản bên trong một < pre> là phần vắn có định dạng giữ nguyên không thay đổi từ trong file html khi ra đến trình duyệt.

## Kiểu HTML
style: Thuộc tính HTML được sử dụng để thêm kiểu vào một phần tử, chẳng hạn như màu sắc, phông chữ, kích thước, v.v.
### Một số thuộc tính và tác dụng 
style           : thuộc tính để tạo kiểu các phần tử HTML vd: < tagname style="property:value;">
background-color: cho màu nền                             vd: < p style="background-color:tomato;">This is a paragraph.< /p>
color           : cho màu văn bản                         vd: < p style="color:red;">This is a paragraph.< /p>
font-family     : cho phông chữ văn bản                   vd: < p style="font-family:courier;">This is a paragraph.< /p>
font-size       : cho các kích thước văn bản              vd: < p style="font-size:160%;">This is a paragraph.< /p>
text-align      : để căn chỉnh văn bản                    vd: < p style="text-align:center;">Centered paragraph.< /p>


## Định dạng văn bản HTML
HTML chứa một số yếu tố để xác định văn bản có ý nghĩa đặc biệt.
### Một số yếu tố định dạng HTML
<b> - Chữ in đậm
<strong> - Văn bản quan trọng
<i> - Văn bản in nghiêng
<em> - Đoạn văn bản được nhấn mạnh
<mark> - Văn bản được đánh dấu
<small> - Văn bản nhỏ hơn
<del> - Văn bản đã xóa
<ins> - Đã chèn văn bản
<sub> - Văn bản chỉ số
<sup> - Văn bản siêu cấp
















