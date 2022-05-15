
<html>
<head>
<title>My Portfolio</title>
<meta charset="utf-8">
<meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1">
<meta name="viewport" content="width=device-width">
<style>
.body {
    background-color: rgb(244, 248, 248);
    min-width: 1200px;
}
/* On smaller screens*/
@media screen and (max-height: 3800px) {
    .sidenav {padding-top: 10px;}
    .sidenav a {font-size: 16px;}
}
#main {
    transition: margin-left .5s;
    padding: 20px;
}
/* The side navigation menu */
.sidenav {
    background-color: rgb(46, 3, 3);
    overflow-x: hidden; 
    padding-top: 60px; 
    transition: 0.5s; 
    height: 100%; 
    width: 0; 
    position: fixed; 
    z-index: 1; 
    top: 0;
    left: 0;
    
}

/* navigation menu */
.sidenav a {
    padding: 8px 8px 8px 32px;
    text-decoration: none;
    display: block;
    font-size: 25px;
    font-family: "Roboto", sans-serif;
    color: #facbcb;
    transition: 0.3s
}

/* hovering color */
.sidenav a:hover, .offcanvas a:focus{
    color: #f1f1f1;
}
.icon-container{
    background-color: rgb(244, 248, 248);
}
/* Position and style of the hambugger button */
.icon {
    position: relative;
    top: 0;
    right: 25px;
    font-size: 36px;
    margin-left: 50px;
    
}

/* Style the accordion */
.accordion {
        background-color: #eee;
        cursor: pointer;
        padding: 8px;
        width: 100%;
        border: 1px solid #000;
        border-bottom: none;
        text-align: left;
        outline: none;
        font-size: 15px;
        transition: 0.4s;
       
    }
    .accordion:last-child{
        border-bottom: 1px solid #000;
    }
    .accordion-header {
        display: flex;
        padding: 16px;
        cursor: pointer;
        
    }
    .accordion-icon {
        width: 16px;
        color: #C00;
    }
    .accordion-title {
        flex: 1;
    }
    .accordion-content {
        padding: 1px;
        background-color: white;
    }
    .accordion-content {
        display: none;
    }
    .active, .accordion:hover {
        background-color: #ccc;
    }
    
* {
  box-sizing: border-box;
}

.column {
  float: left;
  padding: 10px;
 
}

.left {
  width: 30%;
}

.right {
  width: 70%;
}
.row{
    display: none;
}
.row:after {
  content: "";
  display: table;
  clear: both;
}
/* Style for  banner container */
.intro{
    background-image: url('https://images.pexels.com/photos/1229861/pexels-photo-1229861.jpeg?auto=compress&cs=tinysrgb&dpr=1&w=500');
    -webkit-background-size: cover;
	-moz-background-size: cover;
	background-size: cover;
	width: 100%;
	height: 100%;
	min-height: 500px;
	display: table;
	position: relative;
	text-align: center;
}
.intro h1{
    color: white;
    font-size: 50px;
    font-family: "poppins-semibold", serif;
    font-weight: 500;
    font-style: normal;
}
.intro h5 {
	color: #FF0077;
	font-size: 1.6rem;
	line-height: 1.875;
	margin-bottom: 0.3rem;
	letter-spacing: .4rem;
}
.intro-position {
	font-family: "lora-regular", serif;
	font-size: 1.7rem;
	line-height: 2.4rem;
	text-transform: uppercase;
	letter-spacing: .2rem;
	color: #FFFFFF;
	text-shadow: 0 0 6px rgba(0, 0, 0, 0.2);
}
/* Style for about container */
.about{ 
    display: flex;
    flex-direction: column;
    background-color: rgb(244, 248, 248);
    padding: 20px;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

.top{
    display: flex;
    align-items: center;
    margin-bottom: 50px;
}

.skill{
    width: 200px;
    height: 200px;
    contain: content;
}
.skill img{
    width: 100%;
    height: 100%;
}

.top .info{
    display: flex;
    flex-direction: column;
    margin-left: 80px;
}



.bottom{
    display: flex;
    justify-content: space-between;
}

.bottom .left{
    width: 500pX;
}
.bottom .left p{
    margin-bottom: 20px;
    line-height: 1.5;
    font-size: 16px;
}

/*****/
/* Style for  skill container */
.container{
    display: grid;
    grid-template-columns: repeat(2,1fr);
    grid-gap: 1rem;
    margin: 20px ;
}
.container .skill{
    width :         90px;
    height:         90px;
    box-shadow:     3px 3px 4px lightgray;
    cursor:          pointer;
    transition:      ease-in 0.2s;
    display:         flex;
    flex-direction:  column;
    text-align:      center;
    align-items:     center;
    justify-content: center;
    border-radius:   20px;
}
/* Style for  skill container */
.container .skill i{
    font-size:     40px;
    margin-bottom: 10px;
    color:        gray;
    transition:    all ease-in 0.5s;
}

/* Style inputs with type="text", select elements and textareas */
.contact [type=text], select, textarea {
  width: 100%; 
  padding: 12px;
  border: 1px solid #ccc; 
  border-radius: 4px; 
  box-sizing: border-box; 
  margin-top: 6px; 
  margin-bottom: 16px; 
  resize: vertical 
}

/* Style the submit button with a specific background color etc */
.contact input[type=submit] {
  background-color: #04AA6D;
  color: white;
  padding: 12px 20px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}
.contact [type=submit]:hover {
  background-color: #45a049;
}

.contact {
  border-radius: 5px;
  background-color: #f2f2f2;
  padding: 60px;
}
footer {
  text-align: center;
  padding: 3px;
  background-color: rgb(145, 141, 139);
  color: white;
}
</style>

<script>
    /* width of sidebar when opened*/
function openSide() {
    document.getElementById("mySidenav").style.width = "300px";
}

/* width of the side bar when closed */
function closeSide() {
    document.getElementById("mySidenav").style.width = "0";
}
</script>
</head>

<body>

    <body>
        <div id="mySidenav" class="sidenav">
        <a href="javascript:void(0)" class="closebtn" onclick="closeSide()">&times;</a>
        <a href="#about">About</a>
        <a href="#work-experience">Work Experience</a>
        <a href="#projects">Projects</a>
        <a href="#contact">Contact</a>
        </div>
      
      <!-- An Icon to open the side nav-->
      <div class="icon-container">
        <span class="icon" onclick="openSide()"><img src="https://www.clipartmax.com/png/middle/248-2485394_menu-icon-png-red.png" width="40px" ></span>
      </div>
     
      <div>
          <!--intro -->
        <section id="intro">  
            
            <div class="intro">
                <h5>Hello, World.</h5>
            <h1>I'm Ahamed Alshehri.</h1>

            <p class="intro-position">
                <span>Full stack Developer</span>
                <span>Web Application</span> 
            </p>   
            </div>   	
        </section>
         <!-- /intro -->
        <!--About Section-->
        <section id="about" class="about">
            <div class="top">
                <div class="info">
                    <h1>Personal Details</h1>
                    <p>
                        <strong>Name: </strong>Ahamed Alshehri <br>
                        <strong>Date of birth: </strong>17.08.1992 <br>
                        <strong>Work: </strong>Amazon, Seattle <br>
                    </p>
                </div>
    
            </div>
            <div class="bottom">
                <div class="left">
                    <h1>About</h1>
                    <p>
                        Energetic IT technician at an office of over 300 factory employees. 3+ years of experience with factory instruments and office hardware, software, and network connectivity. Increased performance by 5% after spearheading a building-wide OS upgrade. Seeking to leverage wide spectrum of IT knowledge and tech skills to become the next IT technician at Cellubop Gershwin Enterprises.
                    </p>
                    <h1>Education</h1>
                    <strong>BS Computer Science</strong>
		<h1>Github Page:</h1>
                 <strong> <a href="https://github.com/mohammedaljohani1">view my github page</a><strong>
                <div class="right">
                    <h1>Technical Skills</h1>
                    <div class="container">
                        <div class="skill">
                            <img src="data:image/png;base64,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" alt="hero" border="0">
                        </div>
                        <div class="skill">
                        <img src="data:image/png;base64,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" alt="reactjs">
                        </div>
                        <div class="skill">
                            <img src="data:image/png;base64,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" alt="php">
                        </div>        
                        <div class="skill">
                            <img src="https://cdn3.iconfinder.com/data/icons/logos-and-brands-adobe/512/267_Python-512.png" alt="python">
                        </div>  
                        <div class="skill">
                            <img src="data:image/png;base64,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" alt="python">
                        </div>
                        <div class="skill">
                            <img src="data:image/png;base64,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" alt="angular" >
                        </div>
                
                    </div>
                </div>
            </div>
        </section>
        <!--Work Experience section-->      
          <section id="work-experience">
            <h2>Work Experience</h2>
            <div class="accordion">
              <div class="accordion-header">
                <div class="accordion-title"><strong><b>IT Specialist</b>  | January 2019 - December 2021 Amazon, Seattle, WA</strong></div>
                <span class="accordion-icon">+</span>
              </div>
              <div class="accordion-content">
                <h3><b>Key IT Qualifications & Responsibilities</b></h3>
                <ul>
                    <li>Provide technical support to end users and customers</li>
                    <li>Assisted clients with diagnosis of software and hardware issues and concerns.s</li>
                    <li>Coached newly-hired IT specialists on advanced technical procedures.</li>
                    <li>Encouraged timely and relevant upgrades for clients’ products as necessary.</li>
                </ul>
                <h3><b>Key IT Achievements</b></h3>
                <ul>
                    <li>Identified new parts-ordering solution which led to a client wait time reduction of 17% and an increase in client satisfaction by 39%</li>
                    <li>Assisted IT director with administration applications, reducing workload by 19%</li>
                </ul>
              </div>
            </div>
            <div class="accordion">
                <div class="accordion-header">
                  <div class="accordion-title"><strong><b>Help Desk Agent</b> | January 2018 - December 2019 The Kall Center, New York, NY</strong></div>
                  <span class="accordion-icon">+</span>
                </div>
                <div class="accordion-content">
                  <h3><b>Key IT Responsibilities</b></h3>
                  <ul>
                      <li>Coached other help desk support agents on technical duties and managed hardware and software training on product catalog.</li>
                      <li>Encouraged and influenced email and phone clients to make software-pairing decisions based on budget and need.</li>
                      <li>Instituted customer promotional survey to assess software demand, which soon became adopted call center-wide.</li>
                  </ul>
                  <h3><b>Key IT Achievements</b></h3>
                  <ul>
                      <li>Identified ticketing management solution which led to a queue reduction of 18%</li>
                      <li>Assisted IT manager as liaison to clients on software updates, reducing workload by 49%</li>
                  </ul>
                </div>
              </div>
          </section>
          <section id="projects">
	<form style="width:200px;">
            <h2>Projects</h2>
            Select a Project :
            <select id="background" onchange="projectSelector(this)">
              <option  value="projectOne">Dating Application</option>
              <option value="projectTwo">Ecommerce website</option>
              <option value="projectThree">Expense Tracker App</option>
              <option value="projectFour">Car Rental App</option>
            
            </select>
            
            </form>
            <div class="row" id="projectOne" style="display:block;">
                <div class="column left">
                  <h2>Dating Application</h2>
                  <img src="https://i.pinimg.com/736x/d5/d4/42/d5d442915f2a1a99f9ebabb1e1e4fb41.jpg" height="300" width="380" id="springImage">
                </div>
                <div class="column right">
                    <h3>Soulmate Dating App</h3>
                  <p>Soulmate is a  dating app rich in solutions according to the business requirements. This dating app solutions is jammed with comprehensive & attractive features and amazing UI/UX that is appropriate to stay competitive in the market. Being a top dating app development company, we offer an extensive range of services related to dating apps for those who are willing to invest in this sector. With years of experience, our team has provided efficient dating app design & development services to help businesses gain a large customer base. Be it a custom, readymade, or white-label dating application, we provide result-oriented solutions that help businesses to get higher revenue and other profits.</p>
                </div>
              </div>
              
              <div class="row" id="projectTwo">
                <div class="column left">
                  <h2>Ecommerce website</h2>
                  <img src="https://design4users.com/wp-content/uploads/2021/03/website-ecommerce-design.png.pagespeed.ce.UDgKx9BWOo.png" height="300" width="380" id="springImage">
                </div>
                <div class="column right">
                    <h3>EpiMax Shopping Website</h3>
                  <p>Everything starting from the name to the design of this ecommerce website is memorable. You see big bold pictures as part of their web design, with fewer words. If you’re looking for how to design a website in a unique way, you can definitely take some inspiration from The Horse’s amazing website design.</p>
                </div>
              </div>
              <div class="row" id="projectThree">
                <div class="column left">
                  <h2>Expense Tracker App</h2>
                  <img src="https://i.pinimg.com/736x/4f/c9/98/4fc998276ad1c29e69ef83d88243f5c6.jpg" height="300" width="380" id="springImage">
                </div>
                <div class="column right">
                    <h3>ExpeTracker</h3>
                  <p>ExpeTracker has expense-tracking functionality integrated into its app, allowing you to aggregate account balances, track spending and monitor your net worth. While it garners high marks for its functionality, some users are surprised by the number of calls they receive after providing a phone number.</p>
                </div>
              </div>
              <div class="row" id="projectFour">
                <div class="column left">
                  <h2>Car Rental App</h2>
                  <img src="https://i.pinimg.com/originals/bc/b0/b0/bcb0b035c27ccd3d84fca5ddf6cb53c8.png" height="300" width="380" id="springImage">
                </div>
                <div class="column right">
                    <h3>JimCar Rental App</h3>
                  <p>JimCar is one of a few all-in-one solutions for car rental apps. This one covers car rentals along with airplane flights and hotels. You can use an app like this to find bundles on things like rooms, flights, and car rentals to save yourself a few bucks. Additionally, the app has discovery features in case you’re going to a city that you don’t know. We wouldn’t recommend such an app for someone who needs just a car a rental. However, it’s a good solution for those planning a vacation or a business trip somewhere.</p>
                </div>
              </div>
          </section>
          <section id="Contact" class="contact">
              <h1>Contact Me</h1>
            <form action="action_page.php">

            <label for="fname">First Name</label>
            <input type="text" id="fname" name="firstname" placeholder="Your name..">
        
            <label for="lname">Last Name</label>
            <input type="text" id="lname" name="lastname" placeholder="Your last name..">
        
            <label for="country">Country</label>
            <select id="country" name="country">
              <option value="australia">Australia</option>
              <option value="canada">Canada</option>
              <option value="usa">USA</option>
            </select>
        
            <label for="subject">Subject</label>
            <textarea id="subject" name="subject" placeholder="Write something.." style="height:200px"></textarea>
        
            <input type="submit" value="Submit">
        
          </form>
          </section>
          <footer>
            <p>Author: Ahamed Alshehri</p>
            <p><a href="mailto:ahamedalshehri@gmail.com">ahamedalshehri@gmail.com</a></p>
          </footer>
          <script>
    function projectSelector(selectElem) {
      var i = selectElem.selectedIndex;
      if (i < 0) {
       
        return;
      }
    
      var optionValue = selectElem.options[i].value;
    
     
      if (optionValue === "projectOne") {
        document.getElementById('projectOne').style.display = 'block';
        document.getElementById('projectTwo').style.display = 'none';
        document.getElementById('projectThree').style.display = 'none';
        document.getElementById('projectFour').style.display = 'none';
      }
      else if (optionValue === "projectTwo") {;
        document.getElementById('projectOne').style.display = 'none';
        document.getElementById('projectTwo').style.display = 'block';
        document.getElementById('projectThree').style.display = 'none';
        document.getElementById('projectFour').style.display = 'none';
      }
      else if (optionValue === "projectThree") {
        document.getElementById('projectOne').style.display = 'none';
        document.getElementById('projectTwo').style.display = 'none';
        document.getElementById('projectThree').style.display = 'block';
        document.getElementById('projectFour').style.display = 'none';
      }
      else if (optionValue === "projectFour") {
        document.getElementById('projectOne').style.display = 'none';
        document.getElementById('projectTwo').style.display = 'none';
        document.getElementById('projectThree').style.display = 'none';
        document.getElementById('projectFour').style.display = 'block';
      }
      else {
        document.write("Something went wrong. Please refresh.");
      }
    
    
    }
    </script>
          <script>
            const accordionHeader = document.getElementsByClassName('accordion-header');
            const accordionContent = document.getElementsByClassName('accordion-content');
            const accordionIcon = document.getElementsByClassName('accordion-icon');
          for (let i = 0; i < accordionHeader.length; i++) {
            accordionHeader[i].addEventListener('click', function() {
              accordionContent[i].style.display = accordionContent[i].style.display =='block' ? 'none' : 'block';
              accordionIcon[i].innerHTML = accordionContent[i].style.display =='block' ? '-' : '+';  
            });
          }
          </script>
    </div>
</body>
</html>
