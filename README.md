# 15.-Responsive-Website-

## cotainer-fluid replace which "html" and "css"
	<div id="headerContainer" class="row" style="background-color: red;">
		<div class="container" style="background-color: blue;">
			<div class="col-lg-6 headerTitlePart">
				<a title="DanangZ" href="#">
					<img src="styles/images/banner.png" alt="logo">
				</a>
			</div>
		</div>
	</div>
	<div id="container-fluid" class="row" style="background-color: green;">
		<div class="container" style="background-color: blue;">
			<div class="col-lg-6 headerTitlePart">
				<a title="DanangZ" href="#">
					<img src="styles/images/banner.png" alt="logo">
				</a>
			</div>
		</div>
	</div>

/**
 * .header => .headerLeft ... => @media screen and (max-width: * 800px) => .headerRight
 * Notice that: Not using % for margin or padding. 
 * => .banner
 */
 /**
  * @author: lorence
  * @website: lorence@enclave.vn
  */
 .headerContainer{
 	/** Using container-fluid by bootstrap tutorials -- **/
 	width: 100%;
 	overflow: hidden;
 }

