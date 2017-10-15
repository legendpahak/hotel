# hotel
trying repository
<!DOCTYPE html>
<html>
<title>DonaMartaBoutiqueHotel.Home</title>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css">
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css">
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Poppins">

<body>



<!-- leftside menu -->
<?php
require 'menu.php';
?>
<!-- Overlay effect when opening sidebar on small screens -->
<div class="w3-overlay w3-hide-large" onclick="w3_close()" style="cursor:pointer" title="close side menu" id="myOverlay"></div>

<!-- !PAGE CONTENT! -->
<div class="w3-main" style="margin-left:340px;margin-right:40px">
  
  <!-- Login-Click -->
   <div class="w3-container">
  <h2></h2>

  <button onclick="document.getElementById('id01').style.display='block'" class="w3-button w3-green w3-large">Login</button>

  <div id="id01" class="w3-modal">
    <div class="w3-modal-content w3-card-4 w3-animate-zoom" style="max-width:600px">
  
      <div class="w3-center"><br/>
         <img src="img/dona.jpg" alt="Avatar" style="width:30%" class="w3-circle w3-margin-top">
      </div>
        
        
        
        <form  class="w3-container"  method="POST" action="login.php">
      <!--<form class="w3-container" action="reservationfinal.php"> -->
        <div class="w3-section">
        
    <center>
          <label><b>Username</b></label>
          <input type="text" name="username" required><br/>
          <!--<input class="w3-input w3-border w3-margin-bottom" type="text" placeholder="Enter Username" name="usrname" required>-->
          <label><b>Password</b></label>
          <input type="password" name="password" required><br/>
          <!--<input class="w3-input w3-border" type="password" placeholder="Enter Password" name="psw" required>-->
          </center>
      <div class="w3-container w3-border-top w3-padding-16 ">

          <button class="w3-button w3-block w3-green w3-section w3-padding" type="submit" name ="btnlogin">Login</button>
          
          <!--<button class="w3-button w3-block w3-green w3-section w3-padding" type="submit" name ="btnreg" onclick="window.location.href='http://localhost/finalsystem/finalregistration.php'">not yet registered? SIGN UP NOW  </button>-->
      
<input type="button" class="w3-button w3-block w3-green w3-section w3-padding"  value="SIGN UP" onclick="window.location.href='http://localhost/finalsystem/finalregistration.php'" />

        
      
        </div>
        
        
        
        
        
        </div>
        
      

      <div class="w3-container w3-border-top w3-padding-16 w3-light-grey">
        <button onclick="document.getElementById('id01').style.display='none'" type="button" class="w3-button w3-red">Cancel</button>
     
      </div>

    </div>
  </div>
</div>
        
        <!--End of Login box -->
        
        

        
  
 

        
        <!-- Home -- >
            
     <form action="/action_page.php" class="w3-container w3-card-4 w3-light-black w3-text-black w3-margin">
     
  <div class="w3-container" style="margin-top:80px" id="showcase">
    <h1 class="w3-jumbo"><b>Dona Marta Hotel</b></h1>
    
    
    <h1 class="w3-xxxlarge w3-text-red"><b>Introduction</b></h1>
    <hr style="width:50px;border:5px solid red" class="w3-round">
  </div>
  

  <!--end Home -->
  
  <!-- Photo grid (modal) -->

  <div class="w3-row-padding">
    <div class="w3-half">
      <img src=".jpg" style="width:100%" onclick="onClick(this)" alt="">
      <img src="img/dona.jpg" style="width:100%" onclick="onClick(this)" alt=" This property is 1 minute walk from the beach. The beach front of Dona Marta 
     Boutique hotel is located in Tahusan Beach of Southern Leyte. Just 500 m. from 
	 Dona Marta Cave. It has free wifi and free parking. Enjoy the view of the 
	 garden and sea inside the rooms.
     "/>
     <p></p>
       
      <img src="/w3images/diningroom.jpg" style="width:100%" onclick="onClick(this)" alt=" 
      
      Dona Marta Boutique Hotel is a 20 minute boat ride from white beaches of 
	 San Pedro and San Pablo Island. it is a 2 hour, 15 minute drive from 
     	 Tacloban Airport ."/>
    </div>

    <div class="w3-half">
        <img src=".jpg" style="width:100%" onclick="onClick(this)" alt=""/>
        <img src=".jpg" style="width:100%" onclick="onClick(this)" alt=" The air conditioned rooms are equipped with a flat screen TV and an additional 
	 fan. Some rooms have a private patio or sofa bed. En suite bathrooms have a shower."/>
      <img src="/w3images/atrium.jpg" style="width:100%" onclick="onClick(this)" alt=" Guests can rent a bicycle or request for a massage. The hotel can also help 
	 arrange fishing, diving, and cycling excursions. Luggage can be stored at the 24
	 hour front desk. 
	 "/>
      <img src="/w3images/bedroom.jpg" style="width:100%" onclick="onClick(this)" alt="Captains place a restaurants serves a selection of local and continental cuisine.
	 in-room dining is possible with a room service."/>
      <img src="/w3images/livingroom2.jpg" style="width:100%" onclick="onClick(this)" alt=" We speak your langguage !"/>
    </div>
  </div>
  
  <form action="/action_page.php" class="w3-container w3-card-4 w3-light-grey w3-text-blue w3-margin">
  <!-- Modal for full size images on click-->
  <div id="modal01" class="w3-modal w3-black" style="padding-top:0" onclick="this.style.display='none'">
    <span class="w3-button w3-black w3-xxlarge w3-display-topright">×</span>
    <div class="w3-modal-content w3-animate-zoom w3-center w3-transparent w3-padding-64">
      <img id="img01" class="w3-image">
      <p id="caption"></p>
    </div>
  </div>

   
  <!-- Services -->
   
  <div class="w3-container" id="services" style="margin-top:75px">
    <h1 class="w3-xxxlarge w3-text-red"><b>Services.</b></h1>
    <hr style="width:50px;border:5px solid red" class="w3-round"/>
    <div class="w3-row-padding">
    <div class="w3-half">
      <img src="images/index12.jpg" style="width:480px" height="300px" onclick="onClick(this)" alt=""/>
        <h2><b>Outdoors</b></h2>
     <p><b>*Beachfront   *Private Beach Area *Sun Deck  *Private Beach Area<br />*BBQ Facilities *Terrace and   *Private Beach Area    *Grounds</b></p>
    
         <img src="images/index17.jpg" style="width:480px" height="300px" onclick="onClick(this)" alt=""/> 
      <h2><b> Health &  Wellness Facilities</b></h2>
    <p><b> *Message (additional charge)  *Fitness Center Pets *Pets <br />*Pets Are Not</b></p>
     
     <h3><b> Cleanning Services</b></h3>
          <p><b>*Daily Housekeeping, 
     *Ironing Services(additional charges) 
     *Laundry(additional charges</b></p>
           
    </div>

    <div class="w3-half">
        <img src="img/xx.jpg" style="width:480px" height="300px"  onclick="onClick(this)" alt=""/>
         <h2><b>Food & Drinks </b></h2>
     <p><b>*Special Diet Meals (upon request)  *Breakfast in the room  * Internet<br />
      *FREE! Wifi is a available in all ares and free ofcharges *Parking<br />*FREE! Free private parking </b></p>
     
     
                     
           <img src="images/index9.jpg" style="width:480px" height="300px" onclick="onClick(this)" alt=""/>
           <h2><b>General </b></h2>
     <p><b>*Special Diet Meals (upon request)  *Airport Shuttle(additional charges <br />*Shuttle Services(free) *Air Conditioning *Car Rental *Packed Lunches  *Safe</p>
    
    </div>
  </div>
  

 
   
  <!-- Designersrooms -->
  
     
  <div class="w3-container" id="designers" style="margin-top:75px">
    <h1 class="w3-xxxlarge w3-text-red"><b>Rooms</b></h1>
    <hr style="width:50px;border:5px solid red" class="w3-round">
    <p></p>
    <p></p>
    <p><b>Our Rooms are thoughtfully chosen</b>:</p>
  </div>

  <!-- The rooms -->
  <div class="w3-row-padding w3-grayscale">
    <div class="w3-col m4 w3-margin-bottom">
      <div class="w3-light-grey">
        <img src="img/my.jpg" alt="John" style="width:100%">
        <div class="w3-container">
          <h3>Junior Siute</h3>
          <p class="w3-opacity"></p>
          <p>Phasellus eget enim eu lectus faucibus vestibulum. Suspendisse sodales pellentesque elementum.</p>
        </div>
      </div>
    </div>
    <div class="w3-col m4 w3-margin-bottom">
      <div class="w3-light-grey">
        <img src="img/my1.jpg" alt="Jane" style="width:100%">
        <div class="w3-container">
          <h3>Superior Siute</h3>
          <p class="w3-opacity"></p>
          <p>Phasellus eget enim eu lectus faucibus vestibulum. Suspendisse sodales pellentesque elementum.</p>
        </div>
      </div>
    </div>
    <div class="w3-col m4 w3-margin-bottom">
      <div class="w3-light-grey">
        <img src="img/my2.jpg" alt="Mike" style="width:100%">
        <div class="w3-container">
          <h3>Double</h3>
          <p class="w3-opacity"></p>
          <p>Phasellus eget enim eu lectus faucibus vestibulum. Suspendisse sodales pellentesque elementum.</p>
        </div>
      </div>
    </div>
  </div>


  
  
  <!-- Contact

 <div class="w3-container" id="" style="margin-top:75px">
    <h1 class="w3-xxxlarge w3-text-red"><b>Message</b></h1>
    <hr style="width:50px;border:5px solid red" class="w3-round"/>
    <div class="w3-row-padding">
    <div class="w3-half">
 
<div class="w3-row w3-section">
  <div class="w3-col" style="width:50px"><i class="w3-xxlarge fa fa-user"></i></div>
    <div class="w3-rest">
      <input class="w3-input w3-border" name="first" type="text" placeholder="First Name">
    </div>
</div>

<div class="w3-row w3-section">
  <div class="w3-col" style="width:50px"><i class="w3-xxlarge fa fa-user"></i></div>
    <div class="w3-rest">
      <input class="w3-input w3-border" name="last" type="text" placeholder="Last Name">
    </div>
</div>

<div class="w3-row w3-section">
  <div class="w3-col" style="width:50px"><i class="w3-xxlarge fa fa-envelope-o"></i></div>
    <div class="w3-rest">
      <input class="w3-input w3-border" name="email" type="text" placeholder="Email">
    </div>
</div>

<div class="w3-row w3-section">
  <div class="w3-col" style="width:50px"><i class="w3-xxlarge fa fa-phone"></i></div>
    <div class="w3-rest">
      <input class="w3-input w3-border" name="phone" type="text" placeholder="Phone">
    </div>
</div>

<div class="w3-row w3-section">
  <div class="w3-col" style="width:50px"><i class="w3-xxlarge fa fa-pencil"></i></div>
    <div class="w3-rest">
      <input class="w3-input w3-border" name="message" type="text" placeholder="Message">
    </div>
</div>

<p class="w3-center">
<button class="w3-button w3-section w3-blue w3-ripple"> Send </button>
</p>
</form> -->


<!-- End page content -->

<!---AboutAs-->
 <div class="w3-container" id="" style="margin-top:75px">
    <h1 class="w3-xxxlarge w3-text-red"><b>AboutAs</b></h1>
    <hr style="width:50px;border:5px solid red" class="w3-round"/>
    <div class="w3-row-padding">
    <div class="w3-half">
</div>

<div class="w3-container">
  <div style="width:100%">
    <div class="w3-container w3-center">
    <br />
    <br />
      <h1><b>Local Attractions</b></h1>
 <p><b>Unit 508 109 Greenbelt</b></p>
  <p><b>Tahusan Beach, Hinunangan, Southern Leyte, 
  <br/>facing the Pacific Ocean. The off shore Islands of St Peter and St Paul.
   <br/>Rice fields, Crab production, 
   <br/>Snorkelling, Town and Barangay fiestas 
   </b></p>
      <h1><b>ContactAS</b></h1>
      <p><b>Phone  : 0989767543</b></p>
       <p><b>Fax  : 09898879973</b></p>
       
  <br />
  <br />
      
      <div class="w3-section">
      
   
      </div>
    </div>

  </div>
</div>


<script>
// Script to open and close sidebar
function w3_open() {
    document.getElementById("mySidebar").style.display = "block";
    document.getElementById("myOverlay").style.display = "block";
}
 
function w3_close() {
    document.getElementById("mySidebar").style.display = "none";
    document.getElementById("myOverlay").style.display = "none";
}

// Modal Image Gallery
function onClick(element) {
  document.getElementById("img01").src = element.src;
  document.getElementById("modal01").style.display = "block";
  var captionText = document.getElementById("caption");
  captionText.innerHTML = element.alt;
}
</script>


        
        
        
        
        
</div>
</div>       

</body>

</html>

