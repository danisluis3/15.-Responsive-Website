    
    # Media query là gì?

    Như tôi đã giới thiệu ở phần trước Media query là một "công nghệ" được giới thiệu trong Css3. Nguyên tắc nó sử dụng trên thông qua các thông số kích thước màn hình được khai báo thông qua @media
    Với công cụ này chúng ta có thể phân đoạn Css chúng ta ra nhiều phần khác nhau tương ứng với kích thước của các loại thiết bị
    Ví dụ đoạn Css sau áp dụng cho các thiết bị có độ rộng màn hình bé hơn 1024px.

    @media screen and (max-width: 1024px){
        #wrapper{ width: 100%;}
    }

    => Bản chất của RESPONSIVE là sự kết hợp của media query và tính ưu tiên thực thi của Css trên cùng một đối tượng

    # Ví dụ: Thay đổi background của body từ màu trắng => đen=> đỏ của body web khi độ rộng thiết bị thay đổi.
    - Ipad ngang(1024 x 768)
    - Ipad dọc(768 x 1024)
    - Tablet nhỏ(480 x 640)
    - Iphone(480 x 640)
    - Smart phone nhỏ
