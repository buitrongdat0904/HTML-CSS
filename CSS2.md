
## Link trong CSS

Ngoài những cách thông thường để tạo và trang trí đường link mà bạn đã biết trong HTML, thì trong CSS, bạn sẽ có các thuộc tính đa dạng với nhiều giá trị để giúp được link trong Webpage của bạn trở nên đẹp và chuyên nghiệp hơn.

### Tạo link style trong CSS

- Để tạo Link Style, chẳng hạn như tạo màu, font, … cho các đường link trong CSS, bạn có thể sử dụng nhiều thuộc tính CSS đa dạng, 
  ví dụ như color, font-family, background, …
- Ngoài ra, để thiết lập các trạng thái khác nhau cho link, bạn có thể sử dụng các thuộc tính:
- Trạng thái :link – biểu thị rằng trang web này trình duyệt chưa lưu (tức người sử dụng lần đầu tiên click vào đường dẫn này).
- Trạng thái :visited – biểu thị rằng đường dẫn tới trang web này đã được lưu bởi trình duyệt (tức là người sử dụng
  đã click vào đường dẫn này trước đó rồi).
- Trạng thái :hover – biểu thị rằng khi người sử dụng di chuyển chuột qua phần tử mà chứa link đó (tức là phần tử đó là một link
  khi người sử dụng di chuyển chuột qua phần tử đó).
- Trạng thái :active – biểu thị đường link là active khi người sử dụng click chuột vào.
        Ghi chú:
        Trạng thái :hover PHẢI theo sau các trạng thái :link và :visited trong định nghĩa CSS thì mới có hoạt động. Nếu thiếu một trong hai trạng thái trên, thì các Style Rule bạn đã định nghĩa cho :hover sẽ không có giá trị.
        Trạng thái :active PHẢI theo sau trạng thái :hover trong định nghĩa CSS.

### Thiết lập màu cho Link trong CSS
- Để thiết lập màu cho Link, bạn sử dụng thuộc tính color trong CSS. Như đã trình bày trong chương Màu trong CSS, 
  giá trị của thuộc tính color này có thể là tên màu hoặc một giá trị Hex Code, …

### Thiết lập màu cho Visited Link trong CSS
- Trạng thái :visited chỉ rằng đường link này đã được lưu bởi trình duyệt. Để thiết lập màu cho loại đường này, bạn theo dõi ví dụ sau:

        <html>
        <head>
            <style type="text/css">
                a:visited {color: #006600}
            </style>
        </head>
        <body>
            <a href=""> Click vao link nay</a> 
        </body>
        </html> 

Khi bạn click vào đường link này, màu của link sẽ chuyển sang màu xanh lá cây.

## Bảng trong CSS
 
Bảng là một công cụ hiển thị dữ liệu rõ ràng và hiệu quả. Mặc dù với các công nghệ mới (như Kendo UI), thì việc hiển thị dữ 
liệu bằng các thẻ div thường được sử dụng hơn. Tuy nhiên, với các ứng dụng Webpage nhỏ và với lượng dữ liệu hiển thị là 
không lớn thì sử dụng bảng là khá tiện lợi. Chương này sẽ trình bày cách sử dụng các thuộc tính khác nhau 
trong CSS để làm cho bảng của bạn đẹp hơn.

Dưới đây là một số thuộc tính trong CSS:

Thuộc tính **border** được sử dụng để thiết lập đường viền cho bảng.
Thuộc tính **border-collapse** xác định rằng các đường viền của bảng nên được vào hợp thành một đường viền.
Thuộc tính **caption-side** được sử dụng trong phần tử < caption>. Theo mặc định, chúng sẽ được hiển thị ở phần bên trên của bảng. Sử dụng thuộc tính này, bạn có thể xác định vị trí hiển thị của phần tử caption này.
Thuộc tính **empty-cells** xác định xem có hiển thị đường viền không nếu một ô là trống.
Thuộc tính **table-layout** cho phép bạn thiết lập layout cho bảng.

### Thuộc tính border-collapse trong CSS

Thuộc tính này có hai giá trị collapse và separate tương ứng với các đường viền nên được kết hợp với nhau hoặc phân biệt riêng rẽ.

### Độ rộng và chiều cao bảng trong CSS
- Để xác định độ rộng và chiều cao cho bảng, bạn sử dụng hai thuộc tính width và height trong CSS. Hai thuộc tính này 
  có thể nhận các giá trị là % hoặc px.

## Căn chỉnh bảng trong CSS
### Căn chỉnh bảng theo chiều ngang trong CSS

- Bạn sử dụng thuộc tính text-align để xác định sự căn chỉnh nội dung theo chiều ngang của bảng. 
Thuộc tính này có thể nhận các giá trị left, right hoặc center. Ví dụ:

            th {
                text-align: left;
            }

### Căn chỉnh bảng theo chiều dọc trong CSS
- Để căn chỉnh bảng theo chiều dọc, bạn sử dụng thuộc tính vertical-align có thể nhận các giá trị top, bottom, middle.
 Theo mặc định thì nội dung của bảng có căn chỉnh dọc với giá trị middle. Ví dụ:

            td {
                height: 50px;
                vertical-align: bottom;
            }

### Thuộc tính padding trong CSS
- Để điều khiển khoảng cách giữa đường viền và nội dung của bảng, bạn sử dụng thuộc tính padding trong CSS. 
  Giá trị có thể nhận của thuộc tính này là ở dưới dạng đơn vị px.Ví dụ:

            th, td {
                padding: 15px;
                text-align: left;
            }

## Thuộc tính border-spacing trong CSS

- Thuộc tính border-spacing xác định khoảng cách giữa các đường viền của các ô trong bảng. Thuộc tính này có thể nhận một 
  hoặc hai giá trị (có đơn vị là độ dài).
- Nếu cung cấp một giá trị, thì giá trị này sẽ được áp dụng cho đường viền ngang và dọc. Nếu cung cấp hai giá trị, thì tương 
  ứng theo thứ tự sẽ áp dụng cho đường viền ngang và đường viền dọc.

## Thuộc tính caption-side trong CSS

- Theo mặc định, nội dung của thẻ khi được sử dụng trong bảng sẽ được hiển thị bên trên bảng. Tuy nhiên, để thay đổi vị trí này,
  bạn có thể sử dụng thuộc tính caption-side trong CSS.
- Thuộc tính này có thể nhận một trong các giá trị: top, bottom, left, hoặc right. 

## Thuộc tính empty-cells trong CSS
- Để xác định xem có nên hiển thị đường viền cho một ô không có nội dung, bạn có thể sử dụng thuộc tính empty-cells trong CSS.
- Thuộc tính này có thể nhận một trong các giá trị: show, hide hoặc inherit.

## Thuộc tính table-layout trong CSS
- Thuộc tính table-layout hỗ trợ bạn điều khiển cách mà trình duyệt nên tạo layout cho một bảng.
- Thuộc tính này có thể nhận một trong ba giá trị: fixed, auto hoặc inherit.

## Đường viền trong CSS | Border trong CSS

### Thuộc tính border-color trong CSS
- Để xác định màu cho đường viền trong CSS, bạn sử dụng thuộc tính border-color. Ngoài việc xác định màu cho toàn bộ đường viền bao 
quanh phần tử, bạn cũng có thể xác định riêng rẽ màu cho từng phần của đường viền, chẳng hạn như phần trên, đáy, cạnh trái 
hoặc cạnh phải. Tùy theo mục đích, bạn sử dụng một trong các thuộc tính sau đây.

+ Thuộc tính border-bottom-color giúp bạn thay đổi màu của đáy đường viền.
+ Thuộc tính border-top-color giúp bạn thay đổi màu của phần trên đường viền.
+ Thuộc tính border-left-color giúp bạn thay đổi màu của cạnh trái đường viền.
+ Thuộc tính border-right-color giúp bạn thay đổi màu của cạnh phải đường viền.

### Thuộc tính border-style trong CSS
- Để xác định xem style của đường viền là solid, dotted, dashed, double, …, bạn có thể sử dụng thuộc tính border-style trong CSS. 
  Thuộc tính này có thể nhận các giá trị sau:none solid; dotted; dashed; double; groove; ridge; inset; outset; hidden;

- Giống như thuộc tính border-color, bạn cũng có thể xác định style riêng cho từng phần (trên, đáy, cạnh trái, cạnh phải)
  của đường viền. Các thuộc tính là:

+ Thuộc tính border-bottom-style thay đổi style cho cạnh dưới của đường viền.
+ Thuộc tính border-top-style thay đổi style cho cạnh trên của đường viền.
+ Thuộc tính border-left-style thay đổi style cho cạnh trái của đường viền.
+ Thuộc tính border-right-style thay đổi style cho cạnh phải của đường viền.

## Thuộc tính border-width trong CSS

- Sử dụng thuộc tính border-width trong CSS giúp bạn thay đổi độ rộng của đường viền bao quanh một phần tử. Thuộc tính này 
  có thể nhận một giá trị đo chiều dài với đơn vị là px, pt hoặc cm hoặc có thể là thin, medium hoặc thick.

- Để xác định độ rộng cho từng cạnh của đường viền, bạn có thể sử dụng các thuộc tính sau:
+ Thuộc tính border-bottom-width thay đổi style cho cạnh dưới của đường viền.
+ Thuộc tính border-top-width thay đổi style cho cạnh trên của đường viền.
+ Thuộc tính border-left-width thay đổi style cho cạnh trái của đường viền.
+ Thuộc tính border-right-width thay đổi style cho cạnh phải của đường viền.

### Thuộc tính border trong CSS
-Sử dụng thuộc tính border trong CSS, bạn có thể tối thiểu hóa lượng code cần viết mà vẫn có thể xác định đầy đủ style cho đường viền.
-Trong phần style rule xác định cho thuộc tính border, bạn bắt buộc phải xác định giá trị cho thuộc tính border-style.

## Căn lề trong CSS

- Để xác định phần không gian xung quanh các phần tử, bạn sử dụng thuộc tính margin trong CSS. Thuộc tính margin thiết lâp kích cỡ 
  của phần khoảng trống BÊN NGOÀI đường viền. Với margin, bạn cũng có thể xác định một giá trị âm cho thuộc tính này để tạo các phần 
  nội dung gối lên nhau.
- Giá trị của thuộc tính margin không được kế thừa bởi các phần tử con. Bạn hãy nhớ rằng các lề dọc lân cận (các lề trên và lề dưới) 
  sẽ kết hợp thành một lề.
- Để căn lề cho một phần tử, bạn có các thuộc tính sau:
    + Thuộc tính **margin**: sử dụng thuộc tính này bạn có thể thiết lập tất cả style liên quan tới việc căn lề chỉ trong một khai báo CSS.
    + Thuộc tính **margin-bottom** căn lề dưới của một phần tử.
    + Thuộc tính **margin-top** căn lề trên của một phần tử.
    + Thuộc tính **margin-left** căn lề trái của một phần tử.
    + Thuộc tính **margin-right** căn lề phải của một phần tử.

-Tất cả các thuộc tính liên quan tới Margin trên đều có thể nhận các giá trị sau:

+ **auto**: Trình duyệt tự động ước lượng việc căn lề cho phần tử.
+ **length**: Xác định độ rộng (đơn vị px, pt, cm, …) của lề. Giá trị mặc định là 0.
+ **%**: Xác định mối quan hệ giữa lề với độ rộng của phần tử chứa lề.
+ **inherit**: Kế thừa thuộc tính này từ phần tử cha chứa phần tử có thuộc tính margin này.

## List trong CSS

- Trình bày hay liệt kê một danh sách có kèm theo các bullet hoặc dưới dạng đánh số giúp phần văn bản của bạn dễ đọc 
  và tạo cảm giác thân thiện hơn. Để tạo style riêng cho phần list, bạn có thể sử dụng các thuộc tính trong CSS.
- Có 5 thuộc tính trong CSS
    + Thuộc tính **list-style-type** cho phép bạn kiểm soát hình dạng hay bề ngoài của Marker (giống như Bullet) 
      chẳng hạn ở dạng hình tròn, hình vuông, hay dạng số, ...
    + Thuộc tính **list-style-position** xác định rằng marker nên xuất hiện bên trong hay bên ngoài luồng hiển thị nội dung.
    + Thuộc tính **list-style-image:** sử dụng một hình ảnh để làm marker thay cho các bullet hoặc số.
    + Thuộc tính **list-style:** sử dụng thuộc tính này, bạn có thể khai báo một lần
       mà vẫn có thể xác định được tất cả các thuộc tính trên.
    + Thuộc tính **marker-offset** xác định khoảng cách giữa một marker và phần text trong danh sách.
    


