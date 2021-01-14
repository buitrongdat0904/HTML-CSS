
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
        