
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
