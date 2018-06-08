<template>
    <footer class="footer-distributed">
        <div class="footer-left">
            <h3 class="font">Gusto !</h3>
            <p class="footer-links">
                <a href="#">Home</a>
                ·
                <a href="#">Product</a>
                ·
                <a href="#">Team</a>
                ·
                <a href="#">About</a>
            </p>

            <p class="footer-company-name">Gusto Company © 2018</p>
        </div>

        <div class="footer-center">

            <div>
                <span class="logo">&#9872;</span>
                <p><span class="strong">87 Boulevard Pasteur</span> Nice, France</p>
            </div>

            <div>
                <span class="logo">&#9743</span>
                <p>+1 555 123456</p>
            </div>

            <div>
                <span class="logo">&#9993;</span>
                <p><a href="mailto:gusto@ristorante.com">gusto@ristorante.com</a></p>
            </div>

        </div>

        <div class="footer-right">

            <p class="footer-company-about">
                <span>About the company</span>
                Lorem ipsum dolor sit amet, consectateur adispicing elit. Fusce euismod convallis velit, eu auctor lacus vehicula sit amet.
            </p>

            <div class="footer-icons">

                <a href="#">&#9877<i class="fa fa-github"></i></a>
                <a href="#">&#9880<i class="fa fa-facebook"></i></a>
                <a href="#">&#9882<i class="fa fa-twitter"></i></a>
                <a href="#">&#9884<i class="fa fa-linkedin"></i></a>

            </div>

        </div>

    </footer>
</template>

<script>
    export default {
        name: 'Footer'
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

    .footer-distributed{
        background-color: #8C5E58;
        box-shadow: 0 1px 1px 0 rgba(0, 0, 0, 0.12);
        box-sizing: border-box;
        width: 100%;
        text-align: left;
        font: bold 16px sans-serif;

        padding: 55px 50px;
        margin-top: 80px;
    }

    .footer-distributed .footer-left,
    .footer-distributed .footer-center,
    .footer-distributed .footer-right{
        display: inline-block;
        vertical-align: top;
    }

    /* Footer left */

    .footer-distributed .footer-left{
        width: 40%;
    }

    /* The company logo */

    .footer-distributed h3{
        color:  #F4E9CD;
        font: normal 36px 'Anstery', cursive;
        margin: 0;
    }

    /* Footer links */

    .footer-distributed .footer-links{
        color:  #F1F7ED;
        margin: 20px 0 12px;
        padding: 0;
    }

    .footer-distributed .footer-links a{
        display:inline-block;
        line-height: 1.8;
        text-decoration: none;
        color:  inherit;
    }

    .footer-distributed .footer-company-name{
        color:  #54494B;
        font-size: 14px;
        font-weight: normal;
        margin: 0;
    }

    /* Footer Center */

    .footer-distributed .footer-center{
        width: 35%;
    }

    .footer-distributed .footer-center span.logo{
        background-color:  #8C5E58;
        color: #54494B;
        font-size: 25px;
        width: 38px;
        height: 38px;
        border-radius: 50%;
        text-align: center;
        line-height: 42px;
        margin: 10px 15px;
        vertical-align: middle;
    }

    .footer-distributed .footer-center p{
        display: inline-block;
        color: #F1F7ED;
        vertical-align: middle;
        margin:0;
    }

    .footer-distributed .footer-center p span.strong{
        display:block;
        font-weight: normal;
        font-size:14px;
        line-height:2;
    }

    .footer-distributed .footer-center p a{
        color:  #F4E9CD;
        text-decoration: none;;
    }


    /* Footer Right */

    .footer-distributed .footer-right{
        width: 20%;
    }

    .footer-distributed .footer-company-about{
        line-height: 20px;
        color:  #F1F7ED;
        font-size: 13px;
        font-weight: normal;
        margin: 0;
        font-family:  'Avenir', sans-serif;
    }

    .footer-distributed .footer-company-about span{
        display: block;
        color:  #F4E9CD;
        font-size: 28px;
        font-weight: bold;
        margin-bottom: 20px;

        font-family:  'Anstery', sans-serif;
    }

    .footer-distributed .footer-icons{
        margin-top: 25px;
    }

    .footer-distributed .footer-icons a{
        display: inline-block;
        width: 35px;
        height: 35px;
        cursor: pointer;
        background-color:  #54494B;
        border-radius: 2px;

        font-size: 20px;
        color: #ffffff;
        text-align: center;
        line-height: 35px;

        margin-right: 3px;
        margin-bottom: 5px;
    }

    /* If you don't want the footer to be responsive, remove these media queries */

    @media (max-width: 880px) {

        .footer-distributed{
            font: bold 14px sans-serif;
        }

        .footer-distributed .footer-left,
        .footer-distributed .footer-center,
        .footer-distributed .footer-right{
            display: block;
            width: 100%;
            margin-bottom: 40px;
            text-align: center;
        }

        .footer-distributed .footer-center i{
            margin-left: 0;
        }

    }

    @font-face {
        font-family: "Anstery";
        src: url('../font/AnsteryScript.otf');
    }

</style>