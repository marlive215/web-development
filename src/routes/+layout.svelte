<script>

</script>
<main>
    <head>
        <!-- Included link to Google font but does not show up on website for nav links, font in body -->
        <link href='https://fonts.googleapis.com/css?family=Montserrat' rel='stylesheet'>
    </head>
    <body class="page-body">
        <div class="container">
            <nav class="navbar">
                <!-- Where the logo and/or agency name should go -->
                <h1>Agency Name</h1>
                <!-- Links for the navbar -->
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
        font-family: Arial, Helvetica, sans-serif;
        font-size: 18px;
    }

    .container {
        width: 100%;
        height: 80%;
        margin: 0 auto;
        padding: 0px;
        background:black;
    }
    .navbar {
        margin-top: 40px;
        display: flex;
        background: black;
        height: 50px;

        

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
        margin-right: 10px;
    }
    .menu-options li {
        display: inline;
        margin: 0 10px; 
    }

    .list-of-link a {
        text-decoration: none;
        color: white;
        font-size: 20px;
    }
    h1 {
        font-size: 20px;
        font-weight: normal;
        color: #ffff;
    }   
</style>