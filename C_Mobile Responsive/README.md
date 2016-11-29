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

    => Mỗi một cái hình ảnh hiển thị như thế này gọi là một wrapper.
    - Gồm có 2 phần div và có thể thêm thẻ id định nghĩ riêng
    ![alt tag](https://github.com/danisluis3/10.-Responsive-BootStrap-Tutorials/blob/master/13.png)

    => Giải thích đoạn lệnh một tý nhé:

    <div class="titleContainer content" id="advertise">
		<div class="container">
			<h3  class="fadeInUp animated" style="visibility: visible; animation-duration: 1.8s; animation-delay: 3.0s; animation-name: fadeInUp;"> WELCOME TO ADCONNECTER, THE MOUNTAIN OF SUCCESS IS WAITING FOR YOU !</h3>
		</div>
	</div><!-- end titleContainer -->

    + Nếu như bên trong container chứa nhiều nội dung với các định dạng khác nhau thì ta tiến hành đưa vào một thẻ div còn
    duy nhất một nội dung ta trỏ luôn đến component html

