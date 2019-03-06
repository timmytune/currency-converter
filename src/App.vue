<template>
  <div id="app">




  <header style="background-color: rgba(0, 0, 0, 0.6);" id="header">
    <div class="container">

      <div id="logo" class="pull-left">
        <a href="#hero"><img src="img/logo.png" alt="" title="" /></img></a>
        <!-- Uncomment below if you prefer to use a text logo -->
        <!--<h1><a href="#hero">Regna</a></h1>-->
      </div>

      <nav id="nav-menu-container">
        <ul class="nav-menu">
          <li @click="login = 1" ><a href="#hero">Home</a></li>
          <li @click="login = 1"><a href="#about">About Us</a></li>
          <li><a @click="login = 1" href="#services">Services</a></li>
          <li v-if="login"><a @click="login = 3" href="#">Login</a></li>
          <li v-if="!login"><a @click="login = 1" href="#">Logout</a></li>
          <li><a @click="login = 1" href="#contact">Contact Us</a></li>
        </ul>
      </nav><!-- #nav-menu-container -->
    </div>
  </header><!-- #header -->








    <div v-if="login == 1">



  <!--==========================
    Hero Section
  ============================-->
  <section id="hero">
    <div class="hero-container">
      <h1>Welcome to Simple micro</h1>
      <h2>Where micro finance banking is done with ease</h2>
      <a href="#" @click="login = 2" class="btn-get-started">Register</a>
    </div>
  </section><!-- #hero -->

  <main id="main">

    <!--==========================
      About Us Section
    ============================-->
    <section id="about">
      <div class="container">
        <div class="row about-container">

          <div class="col-lg-6 content order-lg-1 order-2">
            <h2 class="title">Few Words About Us</h2>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
            </p>

            <div class="icon-box wow fadeInUp">
              <div class="icon"><i class="fa fa-shopping-bag"></i></div>
              <h4 class="title"><a href="">Eiusmod Tempor</a></h4>
              <p class="description">Et harum quidem rerum facilis est et expedita distinctio. Nam libero tempore, cum soluta nobis est eligendi</p>
            </div>

            <div class="icon-box wow fadeInUp" data-wow-delay="0.2s">
              <div class="icon"><i class="fa fa-photo"></i></div>
              <h4 class="title"><a href="">Magni Dolores</a></h4>
              <p class="description">Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum</p>
            </div>

            <div class="icon-box wow fadeInUp" data-wow-delay="0.4s">
              <div class="icon"><i class="fa fa-bar-chart"></i></div>
              <h4 class="title"><a href="">Dolor Sitema</a></h4>
              <p class="description">Minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat tarad limino ata</p>
            </div>

          </div>

          <div class="col-lg-6 background order-lg-2 order-1 wow fadeInRight"></div>
        </div>

      </div>
    </section><!-- #about -->

    <!--==========================
      Facts Section
    ============================-->
    <section id="facts">
      <div class="container wow fadeIn">
        <div class="section-header">
          <h3 class="section-title">Facts</h3>
          <p class="section-description">Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque</p>
        </div>
        <div class="row counters">

  				<div class="col-lg-3 col-6 text-center">
            <span data-toggle="counter-up">232</span>
            <p>Clients</p>
  				</div>

          <div class="col-lg-3 col-6 text-center">
            <span data-toggle="counter-up">521</span>
            <p>Projects</p>
  				</div>

          <div class="col-lg-3 col-6 text-center">
            <span data-toggle="counter-up">1,463</span>
            <p>Hours Of Support</p>
  				</div>

          <div class="col-lg-3 col-6 text-center">
            <span data-toggle="counter-up">15</span>
            <p>Hard Workers</p>
  				</div>

  			</div>

      </div>
    </section><!-- #facts -->

    <!--==========================
      Services Section
    ============================-->
    <section id="services">
      <div class="container wow fadeIn">
        <div class="section-header">
          <h3 class="section-title">Services</h3>
          <p class="section-description">Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque</p>
        </div>
        <div class="row">
          <div class="col-lg-4 col-md-6 wow fadeInUp" data-wow-delay="0.2s">
            <div class="box">
              <div class="icon"><a href=""><i class="fa fa-desktop"></i></a></div>
              <h4 class="title"><a href="">Lorem Ipsum</a></h4>
              <p class="description">Voluptatum deleniti atque corrupti quos dolores et quas molestias excepturi sint occaecati cupiditate non provident</p>
            </div>
          </div>
          <div class="col-lg-4 col-md-6 wow fadeInUp" data-wow-delay="0.4s">
            <div class="box">
              <div class="icon"><a href=""><i class="fa fa-bar-chart"></i></a></div>
              <h4 class="title"><a href="">Dolor Sitema</a></h4>
              <p class="description">Minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat tarad limino ata</p>
            </div>
          </div>
          <div class="col-lg-4 col-md-6 wow fadeInUp" data-wow-delay="0.6s">
            <div class="box">
              <div class="icon"><a href=""><i class="fa fa-paper-plane"></i></a></div>
              <h4 class="title"><a href="">Sed ut perspiciatis</a></h4>
              <p class="description">Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur</p>
            </div>
          </div>

          <div class="col-lg-4 col-md-6 wow fadeInUp" data-wow-delay="0.2s">
            <div class="box">
              <div class="icon"><a href=""><i class="fa fa-photo"></i></a></div>
              <h4 class="title"><a href="">Magni Dolores</a></h4>
              <p class="description">Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum</p>
            </div>
          </div>
          <div class="col-lg-4 col-md-6 wow fadeInUp" data-wow-delay="0.4s">
            <div class="box">
              <div class="icon"><a href=""><i class="fa fa-road"></i></a></div>
              <h4 class="title"><a href="">Nemo Enim</a></h4>
              <p class="description">At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium voluptatum deleniti atque</p>
            </div>
          </div>
          <div class="col-lg-4 col-md-6 wow fadeInUp" data-wow-delay="0.6s">
            <div class="box">
              <div class="icon"><a href=""><i class="fa fa-shopping-bag"></i></a></div>
              <h4 class="title"><a href="">Eiusmod Tempor</a></h4>
              <p class="description">Et harum quidem rerum facilis est et expedita distinctio. Nam libero tempore, cum soluta nobis est eligendi</p>
            </div>
          </div>
        </div>

      </div>
    </section><!-- #services -->

    <!--==========================
    Call To Action Section
    ============================-->
    <section id="call-to-action">
      <div class="container wow fadeIn">
        <div class="row">
          <div class="col-lg-9 text-center text-lg-left">
            <h3 class="cta-title">Call To Action</h3>
            <p class="cta-text"> Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
          </div>
          <div class="col-lg-3 cta-btn-container text-center">
            <a class="cta-btn align-middle" href="#">Call To Action</a>
          </div>
        </div>

      </div>
    </section><!-- #call-to-action -->

    <!--==========================
      Contact Section
    ============================-->
    <section id="contact">
      <div class="container wow fadeInUp">
        <div class="section-header">
          <h3 class="section-title">Contact</h3>
          <p class="section-description">Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque</p>
        </div>
      </div>

      <!-- Uncomment below if you wan to use dynamic maps -->
      <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d22864.11283411948!2d-73.96468908098944!3d40.630720240038435!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x89c24fa5d33f083b%3A0xc80b8f06e177fe62!2sNew+York%2C+NY%2C+USA!5e0!3m2!1sen!2sbg!4v1540447494452" width="100%" height="380" frameborder="0" style="border:0" allowfullscreen></iframe>

      <div class="container wow fadeInUp mt-5">
        <div class="row justify-content-center">

          <div class="col-lg-3 col-md-4">

            <div class="info">
              <div>
                <i class="fa fa-map-marker"></i>
                <p>A108 Adam Street<br>New York, NY 535022</p>
              </div>

              <div>
                <i class="fa fa-envelope"></i>
                <p>info@example.com</p>
              </div>

              <div>
                <i class="fa fa-phone"></i>
                <p>+1 5589 55488 55s</p>
              </div>
            </div>

            <div class="social-links">
              <a href="#" class="twitter"><i class="fa fa-twitter"></i></a>
              <a href="#" class="facebook"><i class="fa fa-facebook"></i></a>
              <a href="#" class="instagram"><i class="fa fa-instagram"></i></a>
              <a href="#" class="google-plus"><i class="fa fa-google-plus"></i></a>
              <a href="#" class="linkedin"><i class="fa fa-linkedin"></i></a>
            </div>

          </div>

          <div class="col-lg-5 col-md-8">
            <div class="form">
              <div id="sendmessage">Your message has been sent. Thank you!</div>
              <div id="errormessage"></div>
              <form action="" method="post" role="form" class="contactForm">
                <div class="form-group">
                  <input type="text" name="name" class="form-control" id="name" placeholder="Your Name" data-rule="minlen:4" data-msg="Please enter at least 4 chars" />
                  <div class="validation"></div>
                </div>
                <div class="form-group">
                  <input type="email" class="form-control" name="email" id="email" placeholder="Your Email" data-rule="email" data-msg="Please enter a valid email" />
                  <div class="validation"></div>
                </div>
                <div class="form-group">
                  <input type="text" class="form-control" name="subject" id="subject" placeholder="Subject" data-rule="minlen:4" data-msg="Please enter at least 8 chars of subject" />
                  <div class="validation"></div>
                </div>
                <div class="form-group">
                  <textarea class="form-control" name="message" rows="5" data-rule="required" data-msg="Please write something for us" placeholder="Message"></textarea>
                  <div class="validation"></div>
                </div>
                <div class="text-center"><button type="submit">Send Message</button></div>
              </form>
            </div>
          </div>

        </div>

      </div>
    </section><!-- #contact -->

  </main>

 
  <a href="#" class="back-to-top"><i class="fa fa-chevron-up"></i></a>

 



























         </div>


         <div v-if="login == 3">

            

           <section>
             <div style="margin-top: 200px; margin-bottom: 100px;" class="container">


            <h1 style="text-align: center; margin-top: 100px; margin-bottom: 50px;"> Login to the platform </h1>


    <div class="row">
        <div style="margin-left: auto; margin-right: auto;" class="col-6">




  <b-form >
      <b-form-group
        id="exampleInputGroup1"
        label="Email address:"
        label-for="exampleInput1"
        description="We'll never share your email with anyone else."
      >
        <b-form-input
          id="exampleInput1"
          type="email"
          v-model="username"
          required
          placeholder="Enter email" />
      </b-form-group>

      <b-form-group id="exampleInputGroup2" label="Your Password" label-for="exampleInput2">
        <b-form-input
          id="exampleInput2"
          type="password"
          v-model="password"
          required
          placeholder="Enter your password" />
      </b-form-group>

      

   

      <b-button @click="loginer"  variant="primary">Submit</b-button>
      <b-button @click="showregister"  variant="primary">Register</b-button>
    </b-form>


        
        
        
        </div>
    </div>

      </div>
      </section>



    </div>


        <div v-if="login == 2">





           <section>
             <div style="margin-top: 200px; margin-bottom: 100px;" class="container">


            <h1 style="text-align: center; margin-top: 100px; margin-bottom: 50px;"> Register on our platform </h1>


    <div class="row">
        <div style="margin-left: auto; margin-right: auto;" class="col-6">




  <b-form >
      <b-form-group
        id="exampleInputGroup1"
        label="Email address:"
        label-for="exampleInput1"
        description="We'll never share your email with anyone else."
      >
        <b-form-input
          id="exampleInput1"
          type="email"
          v-model="username"
          required
          placeholder="Enter email" />
      </b-form-group>

      <b-form-group id="exampleInputGroup2" label="Your Password" label-for="exampleInput2">
        <b-form-input
          id="exampleInput2"
          type="password"
          v-model="password"
          required
          placeholder="Enter your password" />
      </b-form-group>

      <b-form-group id="exampleInputGroup22" label="Repeat password" label-for="exampleInput22">
        <b-form-input
          id="exampleInput22"
          type="password"
          v-model="password2"
          required
          placeholder="Enter your password again" />
      </b-form-group>

      
      <b-button @click="register"  variant="primary">Register</b-button>
    </b-form>


        
        
        
        </div>
    </div>

      </div>
      </section>







 
    </div>




      <div v-if="!login">
<div class="container">

<div style="margin-top: 200px; margin-bottom: 100px; display block;" class= " row main-container mx-auto">
		<div class="row title-container ">
			<div class="col-md-10">
				<h1 class="title">Currency Converter</h1>
			</div>
			<div class="col-md-2">
				<select class="select-country" @change="updateInputs" v-model="selected">
					<option v-for="country in countries">{{country.name}}</option>
				</select>
			</div>
		</div>
		
		<div class="row">
			<!-- input field 1 -->
			<div class="col-md-6">
				<img style="width: 50px;" class="country-flag" src="https://upload.wikimedia.org/wikipedia/commons/thumb/7/79/Flag_of_Nigeria.svg/255px-Flag_of_Nigeria.svg.png"/>
				<h2 class="country-name">Nigeria</h2>
				<p>Rate: 1 NAIRA</p>
				<input id="currencyInput" class="currency-input" @keyup="calcInput_1" :value="calc2">
			</div>
			<!-- input field 2 -->
			<div class="col-md-6">
				<template v-for="country in countries">
					<template v-if="selected === country.name" v-model="countryRate">
						<img style="width: 50px;" class="country-flag" :src="country.image"/>
						<h2 class="country-name">{{country.name}}</h2>
						<p class="">Rate: {{country.rate}} NAIRA</p>
						<input class="currency-input" @keyup="calcInput_2" :value="calc1"><span>{{country.money}}</span>
					</template>
				</template>
			</div>
		</div>
	</div>

</div>
      </div>








 <!--==========================
    Footer
  ============================-->
  <footer style=" width: 100%; background-color: rgba(0, 0, 0, 0.6); margin-top: 100px;" id="footer">
    <div class="footer-top">
      <div class="container">

      </div>
    </div>

    <div class="container">
      <div class="copyright">
        &copy; Copyright <strong>Simple micro</strong>. All Rights Reserved
      </div>
     
    </div>
  </footer><!-- #footer -->







  </div>
</template>

<script>
import axios from 'axios'
import forIn from 'lodash'
import codes from './currency.js'
import pop from './pop.js'
var store = require('store')


export default {
  name: 'app',
 
  data () {
    return {
      login: 1,
      username: "",
      password: "",
      password2: "",
      
     
    selected: "USA",
		countryRate: 365.0,
		calc1: "",
		calc2: "",
		firstInputSelected: true,
    input: document.getElementById("currencyInput"),
    
		countries: [
			{
				name: "Brazil",
				money: "Reais",
				rate: 150,
				image: "https://s3-us-west-2.amazonaws.com/s.cdpn.io/286148/flag-brazil.png"
			},
			{
				name: "UK",
				money: "Pounds",
				rate: 500.99,
				image: "https://s3-us-west-2.amazonaws.com/s.cdpn.io/286148/flag-uk.png"
			},
			{
				name: "Germany",
				money: "Euro",
				rate: 400,
				image: "https://s3-us-west-2.amazonaws.com/s.cdpn.io/286148/flag-germany.png"
			},
			{
				name: "USA",
				money: "USD",
				rate: 365,
				image: "https://s3-us-west-2.amazonaws.com/s.cdpn.io/286148/flag-usa.png"
			},
			{
				name: "Canada",
				money: "CAD",
				rate: 250.94,
				image: "https://s3-us-west-2.amazonaws.com/s.cdpn.io/286148/flag-canada.png"
			},
			{
				name: "New Zealand",
				money: "NZD",
				rate: 300.09,
				image: "https://s3-us-west-2.amazonaws.com/s.cdpn.io/286148/flag-new-zealand.png"
			},
			{
				name: "Japanese",
				money: "YEN",
				rate: 88.51,
				image: "https://s3-us-west-2.amazonaws.com/s.cdpn.io/286148/flag-japan.png"
      },
      
      {
				name: "Nigeria",
				money: "NIR",
				rate: 1,
				image: "https://upload.wikimedia.org/wikipedia/commons/thumb/7/79/Flag_of_Nigeria.svg/255px-Flag_of_Nigeria.svg.png"
			}
		]
	





      
    }
  },
    methods: {
      getuser(email){
        var user  = {}
        store.get('users').forEach(function(value, key, arr) {
        console.log(key, '==', value)
        if (value.email == email){user = value 
        console.log('got here')}
        } , this)
       return user  
      },
      registeruser(email,password){
            var users = store.get('users')
            if(!users) users = []
            var user = this.getuser(email)
            if(user.email){
              alert("Email already exists in our server")
              return;
            }
            this.login = 0;
            users.push({ email: email, password: password })
            store.set('users', users)
      },
      loginer(){
        var user = this.getuser(this.username)
        if(user.password != this.password){
          user = {};
        }




        if ((this.username == "admin" && this.password == "admin") ||  user.email ){
          this.login = 0;
        }else{
            alert("Incorrect username and password")
        }

      },
      
      logine(){
        this.login = 3

      },

       
        register(){
          if(this.password == this.password2 && this.username && this.password){
          this.registeruser(this.username, this.password)
          
          }else{
          alert("Invalid information")
        }
      },
         showregister(){
          this.login = 2;

      },



      calcInput_1: function(e, rate){
        console.log("----------------------------------------")
			this.calculate(e, rate);
		},
		calcInput_2: function(e, rate){
			this.firstInputSelected = false;
			this.calculate2(e, rate);
		},
		updateInputs: function(){
      var selected;
      var i = 0;
			for(i = 0; i < this.countries.length; i++){
				if(this.selected == this.countries[i].name){
					selected = this.countries[i];
				}
			}
			this.countryRate = selected.rate;
			
			var input2 = parseFloat(document.getElementById("currencyInput").value);
			if(isNaN(input2)){
				this.calc2 = "";
				this.calc1 = "";
				return;
			}
			this.calc1 = (input2 / this.countryRate).toFixed(2);
		},
		calculate: function(e, value){
      var value = parseFloat(e.target.value);
      
			if(isNaN(value)){
				this.calc2 = "";
				this.calc1 = "";
				return;
			}
		
				this.calc2 = value;
				this.calc1 = (value / this.countryRate).toFixed(2);
		
    },
    

    	calculate2: function(e, value){
      var value = parseFloat(e.target.value);
      
			if(isNaN(value)){
				this.calc2 = "";
				this.calc1 = "";
				return;
			}
				this.calc1 = value;
				this.calc2 = (value * this.countryRate).toFixed(2);
			
		}
  }
}
</script>
<style >

body{
	background: #93acd8;
	color: #000;
}

.row{
	width: 100%;
}
.title-container{
	margin-bottom: 25px;
	margin-left: 0;
	text-align: center;

}

	.title{
		margin-right: 15px;
		text-align: left;
		color: #1d2f50;
	}

.select-country{
	width: 100%;
	height: 100%;
	background: white;
}


h2{
	color: #1d2f50;
}

.country-name{
	display: inline-block;
}
.country-flag{
	display: inline-block;
	margin-right: 10px;
	margin-bottom: 12px;
}

.main-container{
	width: 800px;
	position: absolute;
	border-radius: 10px;
	padding: 50px;
	top: 40%;
	left: 50%;
	transform: translate(-50%,-40%);
	background: white;
	
}

.currency-input{
	width: 70%;
	margin-right: 5px;
	font-size: 20px;
	height: 40px;
	border-radius: 5px;
	border: 1px solid #CCC;
	padding-left: 10px;
}




/*
  Theme Name: Regna
  Theme URL: https://bootstrapmade.com/regna-bootstrap-onepage-template/
  Author: BootstrapMade.com
  License: https://bootstrapmade.com/license/
*/
/*--------------------------------------------------------------
# General
--------------------------------------------------------------*/
body {
  background: #fff;
  color: #666666;
  font-family: "Open Sans", sans-serif;
}

a {
  color: #2dc997;
}

a:hover, a:active, a:focus {
  color: #2dca98;
  outline: none;
  text-decoration: none;
}

p {
  padding: 0;
  margin: 0 0 30px 0;
}

h1, h2, h3, h4, h5, h6 {
  font-family: "Poppins", sans-serif;
  font-weight: 400;
  margin: 0 0 20px 0;
  padding: 0;
}

/* Prelaoder */
#preloader {
  position: fixed;
  left: 0;
  top: 0;
  z-index: 999;
  width: 100%;
  height: 100%;
  overflow: visible;
 /* background: #fff url("../img/preloader.svg") no-repeat center center; */
}

/* Back to top button */
.back-to-top {
  position: fixed;
  display: none;
  background: rgba(0, 0, 0, 0.2);
  color: #fff;
  padding: 6px 12px 9px 12px;
  font-size: 16px;
  border-radius: 2px;
  right: 15px;
  bottom: 15px;
  transition: background 0.5s;
}

@media (max-width: 768px) {
  .back-to-top {
    bottom: 15px;
  }
}

.back-to-top:focus {
  background: rgba(0, 0, 0, 0.2);
  color: #fff;
  outline: none;
}

.back-to-top:hover {
  background: #2dc997;
  color: #fff;
}

/*--------------------------------------------------------------
# Header
--------------------------------------------------------------*/
#header {
  padding: 30px 0;
  height: 92px;
  position: fixed;
  left: 0;
  top: 0;
  right: 0;
  transition: all 0.5s;
  z-index: 997;
}

#header #logo {
  float: left;
}

#header #logo h1 {
  font-size: 36px;
  margin: 0;
  padding: 6px 0;
  line-height: 1;
  font-family: "Poppins", sans-serif;
  font-weight: 700;
  letter-spacing: 3px;
  text-transform: uppercase;
}

#header #logo h1 a, #header #logo h1 a:hover {
  color: #fff;
}

#header #logo img {
  padding: 0;
  margin: 0;
}

@media (max-width: 768px) {
  #header #logo h1 {
    font-size: 26px;
  }
  #header #logo img {
    max-height: 40px;
  }
}

#header.header-fixed {
  background: rgba(52, 59, 64, 0.9);
  padding: 20px 0;
  height: 72px;
  transition: all 0.5s;
}

/*--------------------------------------------------------------
# Hero Section
--------------------------------------------------------------*/
#hero {
  width: 100%;
  height: 100vh;
   background: url(https://img.business.com/rc/816x500/aHR0cHM6Ly93d3cuYnVzaW5lc3NuZXdzZGFpbHkuY29tL2ltYWdlcy9pLzAwMC8wMDMvODI4L29yaWdpbmFsL3NodXR0ZXJzdG9ja18xMTU1NDg3ODEuanBn?_ga=2.214877335.1804961063.1551880014-674763242.1551880013) top center;  
  background-size: cover;
  position: relative;
}

@media (min-width: 1024px) {
  #hero {
    background-attachment: fixed;
  }
}

#hero:before {
  content: "";
  background: rgba(0, 0, 0, 0.6);
  position: absolute;
  bottom: 0;
  top: 0;
  left: 0;
  right: 0;
}

#hero .hero-container {
  position: absolute;
  bottom: 0;
  top: 0;
  left: 0;
  right: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  text-align: center;
}

#hero h1 {
  margin: 30px 0 10px 0;
  font-size: 48px;
  font-weight: 700;
  line-height: 56px;
  text-transform: uppercase;
  color: #fff;
}

@media (max-width: 768px) {
  #hero h1 {
    font-size: 28px;
    line-height: 36px;
  }
}

#hero h2 {
  color: #eee;
  margin-bottom: 50px;
  font-size: 24px;
}

@media (max-width: 768px) {
  #hero h2 {
    font-size: 18px;
    line-height: 24px;
    margin-bottom: 30px;
  }
}

#hero .btn-get-started {
  font-family: "Poppins", sans-serif;
  text-transform: uppercase;
  font-weight: 500;
  font-size: 16px;
  letter-spacing: 1px;
  display: inline-block;
  padding: 8px 28px;
  border-radius: 50px;
  transition: 0.5s;
  margin: 10px;
  border: 2px solid #fff;
  color: #fff;
}

#hero .btn-get-started:hover {
  background: #2dc997;
  border: 2px solid #2dc997;
}

/*--------------------------------------------------------------
# Navigation Menu
--------------------------------------------------------------*/
/* Nav Menu Essentials */
.nav-menu, .nav-menu * {
  margin: 0;
  padding: 0;
  list-style: none;
}

.nav-menu ul {
  position: absolute;
  display: none;
  top: 100%;
  left: 0;
  z-index: 99;
}

.nav-menu li {
  position: relative;
  white-space: nowrap;
}

.nav-menu > li {
  float: left;
}

.nav-menu li:hover > ul,
.nav-menu li.sfHover > ul {
  display: block;
}

.nav-menu ul ul {
  top: 0;
  left: 100%;
}

.nav-menu ul li {
  min-width: 180px;
}

/* Nav Menu Arrows */
.sf-arrows .sf-with-ul {
  padding-right: 30px;
}

.sf-arrows .sf-with-ul:after {
  content: "\f107";
  position: absolute;
  right: 15px;
  font-family: FontAwesome;
  font-style: normal;
  font-weight: normal;
}

.sf-arrows ul .sf-with-ul:after {
  content: "\f105";
}

/* Nav Meu Container */
#nav-menu-container {
  float: right;
  margin: 0;
}

@media (max-width: 768px) {
  #nav-menu-container {
    display: none;
  }
}

/* Nav Meu Styling */
.nav-menu a {
  padding: 0 8px 10px 8px;
  text-decoration: none;
  display: inline-block;
  color: #fff;
  font-family: "Poppins", sans-serif;
  font-weight: 400;
  text-transform: uppercase;
  font-size: 13px;
  outline: none;
}

.nav-menu > li {
  margin-left: 10px;
}

.nav-menu > li > a:before {
  content: "";
  position: absolute;
  width: 100%;
  height: 2px;
  bottom: 0;
  left: 0;
  background-color: #2dc997;
  visibility: hidden;
  -webkit-transform: scaleX(0);
  transform: scaleX(0);
  -webkit-transition: all 0.3s ease-in-out 0s;
  transition: all 0.3s ease-in-out 0s;
}

.nav-menu a:hover:before, .nav-menu li:hover > a:before, .nav-menu .menu-active > a:before {
  visibility: visible;
  -webkit-transform: scaleX(1);
  transform: scaleX(1);
}

.nav-menu ul {
  margin: 4px 0 0 0;
  border: 1px solid #e7e7e7;
}

.nav-menu ul li {
  background: #fff;
}

.nav-menu ul li:first-child {
  border-top: 0;
}

.nav-menu ul li a {
  padding: 10px;
  color: #333;
  transition: 0.3s;
  display: block;
  font-size: 13px;
  text-transform: none;
}

.nav-menu ul li a:hover {
  background: #2dc997;
  color: #fff;
}

.nav-menu ul ul {
  margin: 0;
}

/* Mobile Nav Toggle */
#mobile-nav-toggle {
  position: fixed;
  right: 0;
  top: 0;
  z-index: 999;
  margin: 20px 20px 0 0;
  border: 0;
  background: none;
  font-size: 24px;
  display: none;
  transition: all 0.4s;
  outline: none;
  cursor: pointer;
}

#mobile-nav-toggle i {
  color: #fff;
}

@media (max-width: 768px) {
  #mobile-nav-toggle {
    display: inline;
  }
}

/* Mobile Nav Styling */
#mobile-nav {
  position: fixed;
  top: 0;
  padding-top: 18px;
  bottom: 0;
  z-index: 998;
  background: rgba(52, 59, 64, 0.9);
  left: -260px;
  width: 260px;
  overflow-y: auto;
  transition: 0.4s;
}

#mobile-nav ul {
  padding: 0;
  margin: 0;
  list-style: none;
}

#mobile-nav ul li {
  position: relative;
}

#mobile-nav ul li a {
  color: #fff;
  font-size: 16px;
  overflow: hidden;
  padding: 10px 22px 10px 15px;
  position: relative;
  text-decoration: none;
  width: 100%;
  display: block;
  outline: none;
}

#mobile-nav ul li a:hover {
  color: #fff;
}

#mobile-nav ul li li {
  padding-left: 30px;
}

#mobile-nav ul .menu-has-children i {
  position: absolute;
  right: 0;
  z-index: 99;
  padding: 15px;
  cursor: pointer;
  color: #fff;
}

#mobile-nav ul .menu-has-children i.fa-chevron-up {
  color: #2dc997;
}

#mobile-nav ul .menu-item-active {
  color: #2dc997;
}

#mobile-body-overly {
  width: 100%;
  height: 100%;
  z-index: 997;
  top: 0;
  left: 0;
  position: fixed;
  background: rgba(52, 59, 64, 0.9);
  display: none;
}

/* Mobile Nav body classes */
body.mobile-nav-active {
  overflow: hidden;
}

body.mobile-nav-active #mobile-nav {
  left: 0;
}

body.mobile-nav-active #mobile-nav-toggle {
  color: #fff;
}

/*--------------------------------------------------------------
# Sections
--------------------------------------------------------------*/
/* Sections Header
--------------------------------*/
.section-header .section-title {
  font-size: 32px;
  color: #111;
  text-transform: uppercase;
  text-align: center;
  font-weight: 700;
  margin-bottom: 5px;
}

.section-header .section-description {
  text-align: center;
  padding-bottom: 40px;
  color: #999;
}

/* About Us Section
--------------------------------*/
#about {
  background: #fff;
  padding: 80px 0;
}

#about .about-container .background {
  min-height: 300px;
  /*background: url(../img/about-img.jpg) center top no-repeat; */
  margin-bottom: 10px;
}

#about .about-container .content {
  background: #fff;
}

#about .about-container .title {
  color: #333;
  font-weight: 700;
  font-size: 32px;
}

@media (max-width: 768px) {
  #about .about-container .title {
    padding-top: 15px;
  }
}

#about .about-container p {
  line-height: 26px;
}

#about .about-container p:last-child {
  margin-bottom: 0;
}

#about .about-container .icon-box {
  background: #fff;
  background-size: cover;
  padding: 0 0 30px 0;
}

#about .about-container .icon-box .icon {
  float: left;
  background: #fff;
  width: 64px;
  height: 64px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  text-align: center;
  border-radius: 50%;
  border: 2px solid #2dc997;
}

#about .about-container .icon-box .icon i {
  color: #2dc997;
  font-size: 24px;
}

#about .about-container .icon-box .title {
  margin-left: 80px;
  font-weight: 500;
  margin-bottom: 5px;
  font-size: 18px;
  text-transform: uppercase;
}

#about .about-container .icon-box .title a {
  color: #111;
}

#about .about-container .icon-box .description {
  margin-left: 80px;
  line-height: 24px;
  font-size: 14px;
}

/* Facts Section
--------------------------------*/
#facts {
  background: #f7f7f7;
  padding: 80px 0 60px 0;
}

#facts .counters span {
  font-size: 48px;
  display: block;
  color: #2dc997;
}

#facts .counters p {
  padding: 0;
  margin: 0 0 20px 0;
  font-family: "Poppins", sans-serif;
  font-size: 14px;
}

/* Services Section
--------------------------------*/
#services {
  background: #fff;
  background-size: cover;
  padding: 80px 0 60px 0;
}

#services .box {
  padding: 50px 20px;
  margin-bottom: 50px;
  text-align: center;
  border: 1px solid #e6e6e6;
  height: 200px;
  position: relative;
  background: #fafafa;
}

#services .icon {
  position: absolute;
  top: -36px;
  left: calc(50% - 36px);
  transition: 0.2s;
  border-radius: 50%;
  border: 6px solid #fff;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  text-align: center;
  width: 72px;
  height: 72px;
  background: #2dc997;
}

#services .icon a {
  display: inline-block;
}

#services .icon i {
  color: #fff;
  font-size: 24px;
}

#services .box:hover .icon {
  background: #fff;
  border: 2px solid #2dc997;
}

#services .box:hover .icon i {
  color: #2dc997;
}

#services .box:hover .icon a {
  color: #2dc997;
}

#services .title {
  font-weight: 700;
  font-size: 18px;
  margin-bottom: 15px;
  text-transform: uppercase;
}

#services .title a {
  color: #111;
}

#services .description {
  font-size: 14px;
  line-height: 24px;
}

/* Call To Action Section
--------------------------------*/
#call-to-action {
  background: linear-gradient(rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.6));
  background-size: cover;
  padding: 80px 0;
}

#call-to-action .cta-title {
  color: #fff;
  font-size: 28px;
  font-weight: 700;
}

#call-to-action .cta-text {
  color: #fff;
}

@media (min-width: 769px) {
  #call-to-action .cta-btn-container {
    display: flex;
    align-items: center;
    justify-content: flex-end;
  }
}

#call-to-action .cta-btn {
  font-family: "Poppins", sans-serif;
  text-transform: uppercase;
  font-weight: 500;
  font-size: 16px;
  letter-spacing: 1px;
  display: inline-block;
  padding: 8px 30px;
  border-radius: 50px;
  transition: 0.5s;
  margin: 10px;
  border: 2px solid #fff;
  color: #fff;
}

#call-to-action .cta-btn:hover {
  background: #2dc997;
  border: 2px solid #2dc997;
}

/* Portfolio Section
--------------------------------*/
#portfolio {
  background: #f7f7f7;
  padding: 80px 0;
}

#portfolio #portfolio-wrapper {
  padding-right: 15px;
}

#portfolio #portfolio-flters {
  padding: 0;
  margin: 0 0 45px 0;
  list-style: none;
  text-align: center;
}

#portfolio #portfolio-flters li {
  cursor: pointer;
  margin: 0 10px;
  display: inline-block;
  padding: 10px 22px;
  font-size: 12px;
  line-height: 20px;
  color: #666666;
  border-radius: 4px;
  text-transform: uppercase;
  background: #fff;
  margin-bottom: 5px;
  transition: all 0.3s ease-in-out;
}

#portfolio #portfolio-flters li:hover, #portfolio #portfolio-flters li.filter-active {
  background: #2dc997;
  color: #fff;
}

#portfolio .portfolio-item {
  position: relative;
  height: 200px;
  overflow: hidden !important;
  margin-bottom: 15px;
  transition: all 350ms ease;
  transform: scale(1);
}

#portfolio .portfolio-item a {
  display: block;
  margin-right: 15px;
}

#portfolio .portfolio-item img {
  position: relative;
  top: 0;
  transition: all 600ms cubic-bezier(0.645, 0.045, 0.355, 1);
}

#portfolio .portfolio-item .details {
  height: 50px;
  background: #2dc997;
  position: absolute;
  width: 100%;
  height: 50px;
  bottom: -50px;
  transition: all 300ms cubic-bezier(0.645, 0.045, 0.355, 1);
}

#portfolio .portfolio-item .details h4 {
  font-size: 14px;
  font-weight: 700;
  color: #fff;
  padding: 8px 0 2px 8px;
  margin: 0;
}

#portfolio .portfolio-item .details span {
  display: block;
  color: #fff;
  font-size: 13px;
  padding-left: 8px;
}

#portfolio .portfolio-item:hover .details {
  bottom: 0;
}

#portfolio .portfolio-item:hover img {
  top: -30px;
}

/* Team Section
--------------------------------*/
#team {
  background: #fff;
  padding: 80px 0 60px 0;
}

#team .member {
  text-align: center;
  margin-bottom: 20px;
}

#team .member .pic {
  margin-bottom: 15px;
  overflow: hidden;
  height: 260px;
}

#team .member .pic img {
  max-width: 100%;
}

#team .member h4 {
  font-weight: 700;
  margin-bottom: 2px;
  font-size: 18px;
}

#team .member span {
  font-style: italic;
  display: block;
  font-size: 13px;
}

#team .member .social {
  margin-top: 15px;
}

#team .member .social a {
  color: #b3b3b3;
}

#team .member .social a:hover {
  color: #2dc997;
}

#team .member .social i {
  font-size: 18px;
  margin: 0 2px;
}

/* Contact Section
--------------------------------*/
#contact {
  background: #f7f7f7;
  padding: 80px 0 40px 0;
}

#contact #google-map {
  height: 300px;
  margin-bottom: 20px;
}

#contact .info {
  color: #333333;
}

#contact .info i {
  font-size: 32px;
  color: #2dc997;
  float: left;
}

#contact .info p {
  padding: 0 0 10px 50px;
  margin-bottom: 20px;
  line-height: 22px;
  font-size: 14px;
}

#contact .info .email p {
  padding-top: 5px;
}

#contact .social-links {
  padding-bottom: 20px;
}

#contact .social-links a {
  font-size: 18px;
  display: inline-block;
  background: #333;
  color: #fff;
  line-height: 1;
  padding: 8px 0;
  border-radius: 50%;
  text-align: center;
  width: 36px;
  height: 36px;
  transition: 0.3s;
}

#contact .social-links a:hover {
  background: #2dc997;
  color: #fff;
}

#contact .form #sendmessage {
  color: #2dc997;
  border: 1px solid #2dc997;
  display: none;
  text-align: center;
  padding: 15px;
  font-weight: 600;
  margin-bottom: 15px;
}

#contact .form #errormessage {
  color: red;
  display: none;
  border: 1px solid red;
  text-align: center;
  padding: 15px;
  font-weight: 600;
  margin-bottom: 15px;
}

#contact .form #sendmessage.show, #contact .form #errormessage.show, #contact .form .show {
  display: block;
}

#contact .form .validation {
  color: red;
  display: none;
  margin: 0 0 20px;
  font-weight: 400;
  font-size: 13px;
}

#contact .form input, #contact .form textarea {
  border-radius: 0;
  box-shadow: none;
  font-size: 14px;
}

#contact .form button[type="submit"] {
  background: #2dc997;
  border: 0;
  padding: 10px 24px;
  color: #fff;
  transition: 0.4s;
}

#contact .form button[type="submit"]:hover {
  background: #51d8ad;
}

/*--------------------------------------------------------------
# Footer
--------------------------------------------------------------*/
#footer {
  background: #343b40;
  padding: 30px 0;
  color: #fff;
  font-size: 14px;
}

#footer .copyright {
  text-align: center;
}

#footer .credits {
  padding-top: 10px;
  text-align: center;
  font-size: 13px;
  color: #ccc;
}

</style>
