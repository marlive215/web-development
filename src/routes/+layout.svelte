<script>

</script>
<main>
    <body class="page-body">
        <div class="container">
            <nav class="navbar">
                <div class="logo">
                    <h1 class="agency-name"><a href="/">SpyderByte</a></h1>
                </div>
                <div class="menu-options">
                    <ul class="list-of-link">
                        <li><a href="/">Home</a></li>
                        <li><a href="/about">About</a></li>
                        <li><a href="/contact">Contact</a></li>
                        <li><a href="/pricing">Pricing</a></li>
                        <li><a href="/faq">FAQ</a></li>
                    </ul>
                </div>
            </nav>
            <div class="content">
                <div class="url-social-links">
                    <ul class="social-link">
                        <li><a class="social-icons" href="https://www.facebook.com/"><img src="https://img.icons8.com/ios-filled/50/ffffff/facebook.png" width="25" height="25" /></a></li>
                        <li><a class="social-icons" href="https://www.instagram.com/"><img src="https://img.icons8.com/ios-filled/50/ffffff/instagram-new.png" width="25" height="25" /></a></li>
                        <li><a class="social-icons" href="https://www.twitter.com/"><img src="https://img.icons8.com/ios-filled/50/ffffff/twitter.png" width="25" height="25" /></a></li>
                    </ul>
                </div>
            </div>
        </div>
    </body>
</main>







<slot />


<style>
    .page-body {
        margin: 0;
        padding: 0;
        background: #000;
        /*  font won't chnage to Montserrat*/
        font-family: 'Montserrat', sans-serif;
        font-size: 18px;
    }

    .container {
        width: 100%;
        height: 80%;
        margin: 0 auto;
        padding: 0px;
        background:black;
    }

    /* .logo {
        margin-top: 40px;
    } */
    .navbar {
        margin: 0;
        margin-top: 40px;
        flex-grow: 1;
        display: flex;
        background: black;
        height: 100px;
        align-items: center;

        

    }
    .list-of-link {
        display: flex;
        margin-top: 20px;
        padding: 0;
        text-align: center;
        margin-left: auto;
        list-style: none;
        float: none;
        position: absolute;
        top: 6.5%;
        left: 50%;
        transform: translate(-50%, -50%);
        
    }

    .list-of-link li {
        display: inline;
        margin-right: 50px;

    }
    .menu-options li {
        display: inline;
        /* margin: 0 30px;  */
    }

    .list-of-link a {
    text-decoration: none;
    color: white;
    font-size: 20px; 
    font-family: 'Montserrat', sans-serif; 
    font-weight: medium; 
}

    .url-social-links{
        position: absolute;
        right: 40px; 
        bottom: 841.5px;
        transform: translateY(-50%);
        
    }

    .url-social-links a {
        text-decoration: none;
        color: white;
    }

    .url-social-links li {
        display: inline;
    }

    .social-icons {
        font-size: 24px;
    }

    .social-link {
        list-style: none;
        padding: 0;
        margin: 0;
        
    }

    .social-link li {
        display: inline;
        margin-left: 20px;
    }

    .agency-name a {
        text-decoration: none;
        font-size: 30px;
        font-weight: bold;
        color: #ffff; 
       

     }

     .agency-name {
        left: 4000px;
     }

  
</style>