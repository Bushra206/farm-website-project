# farm-website-project[Uploading i<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
    <!--Remix Icons-->
    <link href="https://cdn.jsdelivr.net/npm/remixicon@4.2.0/fonts/remixicon.css"
    rel="stylesheet"/>
</head>
<body>
    <!---------Preloader------->

    <!--------Scroll to Top button-------->

    <!---------Header------->

    <div class="home" id="home">
        <nav>
            <div class="nav-logo">
        <i class="ri-suitcase-line"></i>
        <h2 id="company">OrganicFarm</h2>
            </div>
            <div class="nav-menu" id="nav-menu">
                <ul class="nav-list">
                <li>
                    <a href="#home" class="pages">Home</a>
                </li>
                <li>
                    <a href="#about" class="pages">About</a>
                </li>
                <li>
                    <a href="#featured products" class="pages">Featured Products</a>
                </li>
                <li>
                    <a href="#tour" class="pages">Tour</a>
                </li>
                </ul>
                <div class="nav-close" id="nav-close">
                    <i class="ri-close-line"></i>
                </div>
            </div>
            <!--Toggle dark/light mode later-->
            <i class="ri-moon-line" id="moon"></i>
            <i class="ri-sun-line" id="sun"></i>
            <div class="nav-toggle" id="nav-toggle">
            <i class="ri-apps-line" id="toggle"></i> 
            </div>
            </nav>
            <div class="header" id="header">
                <div class="content">
                    <h2 id="title"><span>Organic</span>Farming</h2>
                    <p>
                        We provide high-quality Organic food products,ranging<br>from vegetables to
                        fruits.We <b>only</b> grow all and sell <br><b>non-GMO</b> products.Check out 
                        more below!
                    </p>
                    <button>Learn More!<i class="ri-arrow-right-line"></i> </button>
                </div>
                <img src="https://www.google.com/url?sa=i&url=https%3A%2F%2Fpikbest.com%2Fpng-images%2Ffruit-and-vegetable-basket_9292613.html&psig=AOvVaw2PYqhF3hsAk8dHouHZUwL_&ust=1713203250072000&source=images&cd=vfe&opi=89978449&ved=0CBIQjRxqFwoTCPDXkMvCw4UDFQAAAAAdAAAAABAS">
                
            </div>
            </div>

</body>
</html>
* {
  margin:0;
  padding:0;
  box-sizing: border-box;
  scroll-behavior: smooth;
  transition: all 0.5s;
}
:root {
    /*FONT SIZES*/
    --largest-font: 112px;
    --lager-font: 70px;
    --large-font: 34px;
    --text-large-font:20px;
    --text-font: 16px;
    /* COLOUR*/
    --text-color:#000;
    --hover-color:#bb3333;
    --dark-color:#095000;
    --bg-color:#b3ffa2;
    --bg-color-header:#b3ffa2d3;
    --header-change-color:#b8eba6d7;
    /*--------MAIN HEADER-------*/
    .home{
        width:100%;
        min-height:100vh;
        display:flex;
        background: var(--bg-color);
        overflow: hidden;
        flex-direction: column;
     }
     nav {
        display: flex;
        position: fixed;
       justify-content: right;
        align-items: center;
        width: 100%;
        padding-right: 120px;
        background-color: var(--bg-color);
        z-index: 10;
        transition: all 0.5s; }
        .nav-logo{
            position: absolute;
            left: 40px;
            top:0;
            justify-content: center;
            align-items: center;
            text-align: center;
            display: flex;
            flex-direction: row;
        }
       .nav-logo i {
        font-size: 1.5em;
        color: var(--dark-color);
        margin:1em;
       }
       #company {
        font-size: var(--text-large-font);
        margin: 1.2em;
        font-family: 'Alkatra';
        padding: 0;
        margin: 20px;
        top: 0;
        cursor: pointer;
        color: var(--dark-color);
        position: absolute;
        left: 40px;
       }
       .nav-menu{
        transition: all 0.5s;
       }
       .nav-menu ul{
        list-style: none;
        display: flex;
        flex-direction:row ;
        justify-content: center;
        transition: all 0.5s ;
       }
       .nav-menu ul li{
        margin: 1.3em 1.5em;
        font-size: var(--text-large-font);
        font-family: 'josefin Sans', 'sans-serif';
        font-weight: 600;
        color: var(--dark-color);
        cursor: pointer;
        transition: all 0.5s;
       }
        .nav-menu ul li :hover{
        color: var(--hover-color);
        transition: all 0.5s;
       }
       .nav-menu ul li a{
        text-decoration: none;
        color: var(--dark-color);
    
       }
       .nav-menu ul li a:hover{
        color: var(--hover-color);
        }
       .nav-toggle{
        display: none;
        visibility: hidden;
        transition: all 0.5s;
       }
       #sun{
        position: absolute;
        top: 0;
        right: 50px;
        margin: 1em;
        display: inline flex;
        visibility: hidden;
        opacity: 0;
        cursor: pointer;
        transition: all 0.5s;
       }
       #moon{
        position: absolute;
        top: 0;
        right: 50px;
        margin: 1em;
        display: inline flex;
        visibility: visible;
        opacity: 1;
        cursor: pointer;
        transition: all 0.5s;
       }
       nav i{
        text-decoration: none;
        color: var(--dark-color);
        font-size: 1.5em;
       }
       .nav-close{
        display: none;
        visibility: hidden;
        transition: all 0.5s;
       }
       @media screen and (max-width: 880px){
        justify-content: center;
        padding-right:0 ;
        width: 100%;
        height: 80px;
        background: var(--bg-color);
        transition: all 0.5s;
    }
    .nav-menu{
        width: 100;
        justify-content: center;
        align-items: center;
        display: block;
        background: var(--bg-color);
        box-shadow: 0 2px 10px var(--header-change-color),0 8px 20px var(--header-change-color);
    }
    .nav-menu ul{
        display: flex;
        flex-direction: column;
        transition: all 0.5s;
    }
    .nav-menu ul li{
        display: flex;
        justify-content: center;
        align-items: center;
        text-align: center;
        flex-direction: row;
    }
    .nav-menu ul li:nth-child(1){
        padding-top: 220px;
    }
    .nav-menu ul li a{
        margin: 4px 20px 0 0;
        align-items: center;
        justify-content: center;
        text-align: center;
    }
    .nav-close{
        display: block;
        visibility: hidden;
        position: absolute;
        font-size: 1.5em;
        top: 18px;
        right: 32px;
        cursor: pointer;
    }
    .nav-toggle{
        position: absolute;
        top: 0;
        margin: 1.6em;
        right: 20px;
        display: inline-flex;
        visibility: visible;
        cursor: pointer;
        transition: all 0.5s;
    }
    #sun #moon{
        margin: 1.1em;
    }
    .header{
        justify-content: center;
        align-items: center;
        display: flex;
        flex-direction: row;
    }
}ndex.html…]()
