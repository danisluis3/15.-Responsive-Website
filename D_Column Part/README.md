[Landing Page]
    - PC first trong Rseponsive
    + PC first là khái niệm để chỉ tuần tự responsive giao diện từ màn hình to xuống màn hình nhỏ
    + Để làm việc với mô hình này chúng ta sử dụng max-width trong media query
    + Dưới đây là các media query điển hình mà ta cần thêm vào dự án
    
    /*Ipad ngang(1024 x 768)*/
    @media screen and (max-width: 1024px){
  
    }
    /*Ipad dọc(768 x 1024)*/
    @media screen and (max-width: 768px){
    
    }
    /*Tablet nhỏ(480 x 640)*/
    @media screen and (max-width: 480px){
    
    }
    /*Iphone(480 x 640)*/
    @media screen and (max-width: 320px){
    
    }
    /*Smart phone nhỏ*/
    @media screen and (max-width: 240px){
    
    }

    Ngoài ra, nếu mình cần responsive trên nhiều thiết bị hơn thì công việc của chúng ta là cần xác 
    định kích thước của nó và thêm vào danh sách media query kia theo thứ tự màn hình to ở trên màn 
    hình nhỏ query ở dưới. Theo cách này thì khi một Selector trong css cần style đi qua từ màn hình
    to đến nhỏ sẽ được thay đổi theo thứ tự ưu tiên. Trái ngược với PC First chúng ta cùng đi qua Mobile First


[WEBSITE => APPLICATION BOOTSTRAP]

    => Mỗi một nội dung 1, 2 và 3 có định dạng là khác nhau, => viết thành 3 thẻ div khác nhau. Riêng với thẻ 
    div thứ 3 ta tiến hành dùng bootstrap để chia cột.

    => Bao bên ngoài 3 thẻ div là thẻ có thuộc tính "container"

    => Theo cách truyền thống.
    <div> có 2 class
    + class đầu tiên định nghĩa width, margin and overflow
    + class thứ hai định nghĩa padding

    => Theo bootstrap 
    <div> có 1 class + n class bootstrap
    => 1 class có nhiệm vụ tích hợp cả margin, padding, width, overflow, khử thuộc tính của bootstrap lên đó

    <div class="ct-part1">
        <h3>About Us</h3>
        <span></span>
    </div>
    <div class="ct-part2">
        <p>If you want to know what adconnecter.com is, and who manages the platform, here you can find some useful information.If you want to know more, please visit our FAQ section.</p>
    </div>
    <div class="ct-part3">
        <!-- Ứng dụng bootstrap để chia cột -->         
    </div>

    => Ứng dụng bootstrap để chia cột. Ở đây ta chỉ dùng thẻ div duy nhất vì các định dạng nội dung của từng div là khác nhau nên ta không
    khai báo một div làm định dạng chung nhé.

    * THÀNH PHẦN BÊN TRONG BOOTSTRAP NÓ LÀ GÌ ???
    - tập hợp nội dung có định dạng giống hay là khác ?
    - viết theo truyền thống hay bootstrap 

    ===> Xem hình 2.png

    <div class="ct-part1">
        <h3>About Us</h3>
        <span></span>
    </div>
    
    <div class="banner-part banner-part1">
        <h3>Do you want to advertise your <br>services and earn money?</h3>
    </div>

    => trường hợp 1: ct-part1 gồm margin,widht, text-align:
    .banner-part{
      width: 100%;
      overflow: hidden;
    }
    .banner-part1 h3{
      margin: 0;
      padding: 0;
      width: 100%;
      display: inline-block;
      text-align: center;
      font-weight: 300;
      color: #fff; 
      text-transform: uppercase;
      font-size: 48px;
      line-height: 62px;
    }

    => trường hợp 2: .banner-part gồm thuộc tính chung cho các div còn lại muốn sử dụng
    .ct-part1{
      width: 100%;
      text-align: center;
      margin-bottom: 20px;
    }
    .ct-part1 h3{
      margin: 0;
      padding: 0;
      width: 100%;
      display: inline-block;
      text-align: center;
      font-weight: 300;
      color: #000; 
      font-size: 36px;
      font-weight: 400;
      margin-bottom: 15px;
    }