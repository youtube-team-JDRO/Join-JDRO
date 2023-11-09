<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>J.D.R.O</title>
    <link rel="icon" href="https://static.wixstatic.com/media/906d00_accddb2993154ccf90cfc4ef09e31654~mv2.png/v1/fill/w_64,h_64,al_c,q_85,usm_0.66_1.00_0.01,enc_auto/906d00_accddb2993154ccf90cfc4ef09e31654~mv2.png" type="imagr/x-icon">
</head>
<body>
    
    <div class="box">
        <div class="form">
            <h2>Join J.D.R.O</h2>
            <form id="myForm">
                <div class="inputbox">
                    <input type="text" value="" id="username" required>
                    <span>username</span>
                </div>
                <div class="inputbox">
                    <input type="email" value="" id="email" required>
                    <span>E-mail</span>
                </div>
                <div class="inputbox">
                    <input type="text" value="" id="phone" required>
                    <span>Phone Number</span>
                </div>
                <div class="inputbox">
                    <input type="text" value="" id="ytlink" required>
                    <span>youtube channel URL</span>
                </div>
                <input type="submit" value="submit" class="sub" id="submit">
            </form>
        </div>
        <div class="text">
        <h5>Welcome to J.D.R.O, the ultimate YouTube community! Our projects have helped many YouTubers just like you to grow their channels and connect with other creators. To join J.D.R.O, simply fill out the form with your YouTube channel link and all other required information.</h5>
    </div>
        <p class="c"><span class="wixui-rich-text__text">© 2023 by<span style="text-decoration:underline;" class="wixui-rich-text__text"><a href="https://www.youtube.com/@ARKA_JDRO" target="_blank" rel="noreferrer noopener" class="wixui-rich-text__text">&nbsp;Arka&nbsp;J.D.R.O</a></span>.</span></p>
    </div>
</body>
<style>
*
{
    margin: 0;
    padding: 0;
    font-family: sans-serif;
    box-sizing: border-box;
}
body
{
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    background-size: cover;
    background-repeat: no-repeat;
}
.box
{
    padding: 20px 30px;
    width: 300px;
    height: 450px;
    backdrop-filter: blur(50px);
    border-radius: 20px;
    background: rgba(49, 49, 49, .2);
    border: 1px solid rgba(54, 255, 245, 0.87);
}
.box .form
{
    padding: 10px 20px;
    color:#3be8ffe0;
    border-radius: 20px;

}
.box .form h2
{
    text-align: center;
    color:#00263b;
    border-radius: 20px;
}
.box .form form
{
    margin-top: 50px;
    align-items: center;
}
.box .form form .inputbox input
{
    padding: 10px 20px;
    border: none;
    outline: none;
    background: none;
    border-bottom: 1px solid #12151e;
    margin-bottom: 30px;
    color: #fff;
}
.box .form form .inputbox span
{
    position: absolute;
    transform: translateY(-80px);
    font-size: 14px;
    color: #fff;
}
.box .form form .sub
{
    padding: 10px 20px;
    color: #fff;
    border: none;
    outline: none;
    background: #000000;
    cursor: pointer;
    font-size: 16px;
    border-radius: 50px;
    transition:transform 0.2s ease;
    
}
.box .form form .sub:hover {
    background-color: #222222;
}
.box .form form .sub:active{
    transform: scale(0.96);
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
    
    
}
a{
    color: rgba(0, 78, 83, 0.808);
    
      
}
picture{
    padding-bottom: 600px;
    padding-top: 20px;
    
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
    background: rgba(149, 230, 255, 0.24); 
    border-radius: 10px;
  }
  
  /* Handle on hover */
  ::-webkit-scrollbar-thumb:hover {
    background: #2ffff5; 
  }


</style>
<script type="module">
  import { initializeApp } from "https://www.gstatic.com/firebasejs/9.19.1/firebase-app.js";
  import { getDatabase, ref, set } from "https://www.gstatic.com/firebasejs/9.19.1/firebase-database.js";

  const firebaseConfig = {
    apiKey: "AIzaSyAMVh-7r38ztZyfv99HIRXLnxtSqBHxQmU",
    authDomain: "joinjdro.firebaseapp.com",
    projectId: "joinjdro",
    storageBucket: "joinjdro.appspot.com",
    messagingSenderId: "435388746666",
    appId: "1:435388746666:web:a817482cd2f6a9ae8379d3"
  };

  const app = initializeApp(firebaseConfig);
  const db = getDatabase(app);


document.getElementById("myForm").addEventListener('submit', function(e) {
  e.preventDefault();

  const username = document.getElementById("username").value;
  const email = document.getElementById("email").value;
  const phone = document.getElementById("phone").value;
  const ytlink = document.getElementById("ytlink").value;

  if (!username || !email || !phone || !ytlink) {
    alert("Fill up the form first.");
    return; // Stop the submission if any field is empty
  }

  const userData = {
    username,
    email,
    PhoneNumber: phone,
    YoutubrURL: ytlink
  };

  set(ref(db, 'user/' + username), userData)
    .then(() => {
      alert("Login Successful!");
      document.getElementById("myForm").reset(); // Reset the form
    })
    .catch((error) => {
      console.error("Error adding document: ", error);
      alert("An error occurred. Please try again later.");
    });
});

</script>
</html>
