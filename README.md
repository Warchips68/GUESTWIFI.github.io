!DOCTYPE html>
<html>

<head>
    <title id="title"></title>
    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8" />
    <meta name="theme-color" content="#d0d2d6" />
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="stylesheet" href="css/style.css">
    <link rel="stylesheet" href="css/bg.css">
    <link rel="stylesheet" type="text/css" href="css/vanzj.css">
    <script defer src="js/vanzj.js"></script>

</head>

<body>
    <audio autoplay loop>
       <source src="audio/music.mp3"> 
    </audio>

    <div id="grid"></div>
       
  <div class="bg">
    
        $(if chap-id)
        <form name="sendin" action="$(link-login-only)" method="post">
            <input type="hidden" name="username" />
            <input type="hidden" name="password" />
            <input type="hidden" name="dst" value="$(link-orig)" />
            <input type="hidden" name="popup" value="true" />
        </form>

        <script type="text/javascript" src="md5.js"></script>
        <script type="text/javascript">
            function doLogin() {
                document.sendin.username.value = document.login.username.value;
                document.sendin.password.value = hexMD5('$(chap-id)' + document.login.password.value +
                    '$(chap-challenge)');
                document.sendin.submit();
                return false;
            }
        </script>
        $(endif)
          
            <div id="main" class="main">
            <div class="box">

                <!--Below line is the Wifi Name Text-->
                    <i style="font-size:80px; text-align: right; margin-left: 210px; margin-bottom: -150px; color: #fafafa; text-shadow: 0 10px 15px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);" class="icon icon-rss">&#xf09e;</i><br>
                    <font style="font-size:40px; color: #fffffa; text-shadow: 0 10px 15px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19); margin-top: -150px;"><b>Vanz J Tutorials</b></font>
                <!--Above line is the Wifi Name Text-->
            
            </div>
            <div class="container">

                <!--Below line is the Running Banner Text-->
                <marquee HSPACE="-45" vspace="" behavior="" height="20" text-align=bottom><font color=#ffffff>
                    <div>Welcome to the login portal&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;||&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Enjoy the unlimited data surfing, online gaming, streaming and downloading!&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;||&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Stay at home! Stay safe always.</div>
                </font></marquee>
                <!--Above line is the Running Banner Text-->
                <br>

                <!--Sliding Picture Start-->
                <div class="slidingImage">
                    <div class="slider">
                        <div class="slides">
                            <input type="radio" name="radio-btn" id="radio1">
                            <input type="radio" name="radio-btn" id="radio2">
                            <input type="radio" name="radio-btn" id="radio3">
                            <input type="radio" name="radio-btn" id="radio4">
                            <input type="radio" name="radio-btn" id="radio5">

                            <div class="slide first">
                                <img src="img/1.jpg">
                            </div>
                            <div class="slide">
                                <img src="img/2.jpg">
                            </div>
                            <div class="slide">
                                <img src="img/3.jpg">
                            </div>
                            <div class="slide">
                                <img src="img/4.jpg">
                            </div>
                            <div class="slide">
                                <img src="img/5.jpg">
                            </div>

                            <div class="navigation-auto">
                                <div class="auto-btn1"></div>
                                <div class="auto-btn2"></div>
                                <div class="auto-btn3"></div>
                                <div class="auto-btn4"></div>
                                <div class="auto-btn5"></div>
                            </div>
                        </div>
                        
                    </div>

                    <script type="text/javascript">
                        var counter=1;
                        setInterval(function(){
                            document.getElementById('radio' + counter).checked =true;
                            counter++;
                            if (counter > 5){
                                counter = 1;
                                setInterval=1000;
                                
                            }
                        },3000);
                    </script>
                </div>
                <!--Sliding Picture End-->              


                <br>



            <div class="box">
                <button id="btnvrc" class="small-button" onclick="voucher();"><i class="icon icon-ticket">&#xf145;</i>Voucher</button>
                <button id="btnmem" class="small-button" onclick="member();"><i class="icon icon-user">&#xe80f;</i>User/Password</button>
                
            </div>
            <div class="blinking" id="infologin"></div>

            <form autocomplete="off" name="login" action="$(link-login-only)" method="post" $(if chap-id) onSubmit="return doLogin()"
                $(endif)>
                <input type="hidden" name="dst" value="$(link-orig)" />
                <input type="hidden" name="popup" value="true" />
                <input class="username" name="username" type="text" value="$(username)" />
                <input class="password" name="password" placeholder="Password" type="hidden" />
                $(if error)<div class="notice">$(error)</div>$(endif)
                <button class="button" type="submit">Connect</button>

            </form>
            <br>

            $(if trial == 'yes')
            <div class="trialText">Try it for free, <a style="text-decoration: underline; color:#ffffff;" href="$(link-login-only)?dst=$(link-orig-esc)&amp;username=T-$(mac-esc)">just click here</a></div>
            $(endif)
                <br />
            <div>
                <table class="table3">
                    <caption style="font-size: 16px; font-weight: bold;">WIFI RATES</caption>
                    <tr>
                        <th width="33%">Package</th>
                        <th width="33%">Time</th>
                        <th width="33%">Price</th>
                    </tr>
                    <tr>
                        <td>1</td>
                        <td>1 hour</td>
                        <td>₱ 5.00</td>
                    </tr>
                    <tr>
                        <td>2</td>
                        <td>3 hours</td>
                        <td>₱ 10.00</td>
                    </tr>
                    <tr>
                        <td>3</td>
                        <td>1 day</td>
                        <td>₱ 20.00</td>
                    </tr>
                    <tr>
                        <td>4</td>
                        <td>2 days</td>
                        <td>₱ 30.00</td>
                    </tr>
                    <tr>
                        <td>5</td>
                        <td>1 month</td>
                        <td>₱ 200.00</td>
                    </tr>
                </table>
                <br>
                <div>
                    <!--font class="blinking1" color=#4B4B46>For more info & queries please feel free to email vanzj.tutorials@gmail.com or you may contact cel.# 0977 444 8888.</font-->
                </div>
        </div>
        </div>
        <br><br>
        <div class="box" style="color:white;">

        <i>Powered by</i> <a href="https://www.youtube.com/c/VanzJTutorials" style="color: #c40c06;"><b>Vanz J Tutorials</b></a>
            
        </div>
        </div>

<script type="text/javascript" src="md51.js"></script>

<script type="text/javascript">
var hostname = window.location.hostname;
document.getElementById('title').innerHTML = hostname  + " > login";

document.login.username.focus();

var infologin = document.getElementById('infologin');
infologin.innerHTML = "Enter the Voucher Code then click Connect";

// login page 2
var username = document.login.username;
var password = document.login.password;

username.placeholder = "Voucher Code";

// set password = username
function setpass() {
    var user = username.value
    //user = user.toLowerCase();
    username.value = user;
    password.value = user;
}

username.onkeyup = setpass;

// change to voucher mode
function voucher() {
    username.focus();
    username.onkeyup = setpass;
    username.placeholder = "Voucher Code";
    username.style = "border-radius:3px;"
    password.type = "hidden";
    infologin.innerHTML = "Enter the Voucher Code then click Connect";
}

// change to member mode
function member() {
    username.focus();
    username.onkeyup = "";
    username.placeholder = "Username";
    username.style = "border-radius:3px 3px 0px 0px;"
    password.type = "password";
    infologin.innerHTML = "Enter Username & Password then click Connect";
}
</script>

</body>

</html>
