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

    <nav class="headerContainer navbar navbar-default navbar-fixed-top">
    => tạo ra một div thiết lập css [width,margin,overflow,..]
    => tạo ra div 2 là định dạng padding cho nội dung chứa bên trong 
    * Vì bootstrap hổ trợ thanh nằm trên => navbar => ứng dụng vào + các thuộc tính loại navbar 

    <div class="navbar-header">
        <button type="button" class="navbar-toggle">
		    <span class="icon-bar"></span>
		    <span class="icon-bar"></span>
		    <span class="icon-bar"></span>
	    </button>
        <a href="" title="" id="logo" class="navbar-brand"><img src="styles/images/logo.png" alt="home"></a>
    </div>
    => Chỉ dụng navbar-header => hổ trợ cho chúng ta thiết lập vị trí nội dung này, cần css định nghĩa đó là 
    div thứ 2 là không cần

    <div>
        <div class="navRight navbar-collapse collapse" id="myNavbar">
			<ul class="navRightLeft nav navbar-nav navbar-right">
				<li><a href="#myPage" data-click="scroll-to-target">Home</a></li>
				<li><a href="#advertise" data-click="scroll-to-target">advertise</a></li>
				<li><a href="#earn" data-click="scroll-to-target">earn</a></li>
				<li><a href="#payments" data-click="scroll-to-target">payments</a></li>
				<li><a href="#forum" data-click="scroll-to-target">forum</a></li>
				<li><a href="#faq" data-click="scroll-to-target">FAQ</a></li>
				<li><a href="#support" data-click="scroll-to-target">support</a></li>
				<li><a href="#" id="login" data-click="scroll-to-target">login</a></li>
				<li><a href="#" id="signup" data-click="scroll-to-target">signup</a></li>
			</ul>
		</div>
    </div>
    => Bootstrap hổ trợ chúng ta rồi nên ta không cần đặt vào thay vì đó dùng thuộc tính bootstrap luôn ăn theo

    * navbar
    => navbar-default navbar-fixed-top
    => navbar-header
    => navbar-toggle
    => navbar-collapse

    * Nếu trên cùng thẻ div thể hiện các thuộc tính bootstrap thì ta có thể định nghĩa lại bằng cách thêm class hoặc id
    * Nếu như đã sử dụng bootstrap hãy đặt riêng khối div để hiển thị tốt nhất
