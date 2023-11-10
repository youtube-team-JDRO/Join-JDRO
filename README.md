<!DOCTYPE html>
<!-- code by webdevtrick ( https://webdevtrick.com ) -->
<html>

<head>
  <meta charset="UTF-8">
  <title>Responsive Dropdown nav-bar Bar</title>
	<link href="https://fonts.googleapis.com/css?family=Righteous&display=swap" rel="stylesheet">
      <link rel="stylesheet" href="style.css"> 
</head>

<body>

  <section class="nav-bar">
  <div class="nav-container">
    <div class="brand">
      <a href="https://youtube-team-jdro.github.io/Join-JDRO/"><img src="https://static.wixstatic.com/media/906d00_accddb2993154ccf90cfc4ef09e31654~mv2.png/v1/fill/w_64,h_64,al_c,q_85,usm_0.66_1.00_0.01,enc_auto/906d00_accddb2993154ccf90cfc4ef09e31654~mv2.png" style="width: 50px; margin-top: 10px; "></a>
    </div>
    <nav>
      <div class="nav-mobile"><a id="nav-toggle" href="#!"><span></span></a></div>
      <ul class="nav-list">
        <li>
          <a href="https://youtube-team-jdro.github.io/Join-JDRO/">Home</a>
        </li>
        <li>
          <a href="#!">Social Mideas</a>
			    <ul class="nav-dropdown">
            <li>
              <a href="https://instagram.com/arka_j.d.r.o?igshid=ZDdkNTZiNTM=">Instragram</a>
            </li>
            <li>
              <a href="https://www.facebook.com/arindam.paul.528">Facebook</a>
            </li>
            <li>
              <a href="https://twitter.com/ArkaJDRO1?t=tXl22IuS6Hp0LutUsbDsTQ&s=08">Twitter </a>
            </li>
            <li>
              <a href="https://www.youtube.com/@ARKA_JDRO">Youtube</a>
            </li>
          </ul>
        </li>
        <li>
          <a href="https://youtube-team-jdro.github.io/Join-JDRO/Join.html">Join JDRO</a>
        </li>
        <li>
          <a href="https://whatsapp.com/channel/0029Va8reGt05MUW8kekI83p">WhatsApp </a>
        </li>
        <li>
          <a href="https://youtube-team-jdro.github.io/Join-JDRO/contact.html">Contact Us </a>
        </li>
      </ul>
    </nav>
  </div>
</section>

  <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/2.1.3/jquery.min.js"></script>

<h1 style="text-align: center; font-family: Arial, Helvetica, sans-serif;">J.D.R.O</h1>
<hr style="color: rgba(1, 189, 189, 0.808);">
<div style=" border-radius: 20px;
background-color: #81f0ff38;
  padding: 30px ; padding-inline: 20px;">
<h5>Welcome to J.D.R.O, a vibrant YouTube community dedicated to creating a wide range of engaging content, from the fascinating world of sigma to various other exciting subjects. To become a part of our creative family, all you need is a YouTube channel and a minimum of 5 subscribers. Whether you're an aspiring content creator or a passionate viewer, J.D.R.O is the place where like-minded individuals come together to share, explore, and celebrate the diverse world of online content. Join us on this exciting journey as we inspire and connect through the power of digital storytelling.</h5>
 <div class="mydiv">
  <a href="https://youtube-team-jdro.github.io/Join-JDRO/Join.html">
  <button>JOIN</button>
  </a>
</div> 
  <h5>If you are interested in music you can check this vodeos </h5>
<div class="if">
<iframe width="460" height="250"  src="https://www.youtube.com/embed/XyfuYSy3beQ?si=fDS-1OPvWrXJ78jC" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen style="border-radius: 10px;  "></iframe>
<iframe width="460" height="250" src="https://www.youtube.com/embed/ArCeEW79Keo?si=bAYYShvjRns2Tu_B" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen style="border-radius: 10px;" > </iframe>
</div>
<div class="mydiv">
  <a href="https://youtube-team-jdro.github.io/Join-JDRO/contact.html">
  <button>Contact</button>
  </a>
</div>
</div>

<p class="c"><span class="wixui-rich-text__text">© 2023 by<span style="text-decoration:underline;" class="wixui-rich-text__text"><a href="https://www.youtube.com/@ARKA_JDRO" target="_blank" rel="noreferrer noopener" class="wixui-rich-text__text">&nbsp;Arka&nbsp;J.D.R.O</a></span>.</span></p>
  







</body>
<style>
body {
	margin: 0;
	padding: 0;
}

.nav-bar {
  height: 70px;
  background: #262626;
}

.brand {
  position: absolute;
  padding-left: 20px;
  float: left;
  line-height: 70px;
  text-transform: uppercase;
  font-size: 1.4em;
  
}
.brand a img {
	max-height: 70px;
}
.brand a,
.brand a:visited {
  color: #ffffff;
  text-decoration: none;
}

.nav-container {
  max-width: 1000px;
  margin: 0 auto;
}

nav {
  float: right;
}
nav ul {
  list-style: none;
  margin: 0;
  padding: 0;
  font-family: Arial, Helvetica, sans-serif;
}
nav ul li {
  float: left;
  position: relative;
  transition: 0.3s;
  
}
nav ul li a,
nav ul li a:visited {
  display: block;
  padding: 0 20px;
  line-height: 70px;
  background: #262626;
  color: #ffffff;
  text-decoration: none;
}
nav ul li a:hover,
nav ul li a:visited:hover {
  background: #0c3e49;
  color: #ffffff;
}
nav ul li a:not(:only-child):after,
nav ul li a:visited:not(:only-child):after {
  padding-left: 4px;
  content: ' ▾';
}
nav ul li ul li {
  min-width: 190px;
}
nav ul li ul li a {
  padding: 15px;
  line-height: 20px;
}

.nav-dropdown {
  position: absolute;
  display: none;
  z-index: 1;
  box-shadow: 0 3px 12px rgba(0, 0, 0, 0.15);
}
.nav-mobile {
  display: none;
  position: absolute;
  top: 0;
  right: 0;
  background: #262626;
  height: 70px;
  width: 70px;
}

@media only screen and (max-width: 798px) {
  .nav-mobile {
    display: block;
  }

  nav {
    width: 100%;
    padding: 70px 0 15px;
  }
  nav ul {
    display: none;
  }
  nav ul li {
    float: none;
  }
  nav ul li a {
    padding: 15px;
    line-height: 20px;
	padding-left: 25%;
	 
  }
  nav ul li ul li a {
    padding-left: 30%;
  }

  .nav-dropdown {
    position: static;
  }
	.brand a img {
		max-height: 60px;
		margin-top: 5px;
	}
}
@media screen and (min-width: 799px) {
  .nav-list {
    display: block !important;
  }
}
#nav-toggle {
  position: absolute;
  left: 18px;
  top: 22px;
  cursor: pointer;
  padding: 10px 35px 16px 0px;
}
#nav-toggle span,
#nav-toggle span:before,
#nav-toggle span:after {
  cursor: pointer;
  border-radius: 1px;
  height: 5px;
  width: 35px;
  background: #ffffff;
  position: absolute;
  display: block;
  content: '';
  transition: all 300ms ease-in-out;
}
#nav-toggle span:before {
  top: -10px;
}
#nav-toggle span:after {
  bottom: -10px;
}
#nav-toggle.active span {
  background-color: transparent;
}
#nav-toggle.active span:before, #nav-toggle.active span:after {
  top: 0;
}
#nav-toggle.active span:before {
  transform: rotate(45deg);
}
#nav-toggle.active span:after {
  transform: rotate(-45deg);
}

article {
  max-width: 1000px;
  margin: 0 auto;
  padding: 10px;
}

h5{
  font-family: worksans-semibold,"work sans",sans-serif !important;
    font-size: calc((4.634 * var(--one-unit)) - (var(--scrollbar-width) * 0.046340000000000006)) !important;
    font-style: normal !important;
    text-decoration: none !important;
    text-align: center !important;
    padding-top: 100px;
    padding-bottom: 50px;
}

p{
    font-size: 14px;
    text-align: center;
    color: rgba(0, 78, 83, 0.808);
    padding-bottom: 30px;
    font-family: Arial, Helvetica, sans-serif;


}
a{
    color: rgba(0, 78, 83, 0.808);
    font-family: Arial, Helvetica, sans-serif;
}
button{
  padding: 10px 20px;
    color: #fff;
    border: none;
    outline: none;
    background: #000000;
    cursor: pointer;
    font-size: 16px;
    border-radius: 50px;
    transition:transform 0.2s ease;
    width: 100px;
    
}
button:hover{
  background-color: #222222;
}
button:active{
  transform: scale(0.96);
}

/* width */
::-webkit-scrollbar {
    width: 7px;
  }

  /* Track */
  ::-webkit-scrollbar-track {
    box-shadow: inset 0 0 5px rgb(255, 255, 255); 
    border-radius: 10px;

  }

  /* Handle */
  ::-webkit-scrollbar-thumb {
    background: rgba(94, 145, 160, 0.24); 
    border-radius: 10px;
  }

  /* Handle on hover */
  ::-webkit-scrollbar-thumb:hover {
    background: #2ffff5; 
  }

  .mydiv{
    text-align: center;
    padding-top: 40px;
  }
  .if{
    text-align: center;
  }
</style>

<script>
(function($) { 
  $(function() { 
    $('nav ul li a:not(:only-child)').click(function(e) {
      $(this).siblings('.nav-dropdown').toggle();
      $('.dropdown').not($(this).siblings()).hide();
      e.stopPropagation();
    });
    $('html').click(function() {
      $('.nav-dropdown').hide();
    });
    $('#nav-toggle').click(function() {
      $('nav ul').slideToggle();
    });
    $('#nav-toggle').on('click', function() {
      this.classList.toggle('active');
    });
  }); 
})(jQuery);

</script>
</html>
