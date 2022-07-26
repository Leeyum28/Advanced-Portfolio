# Advanced-Portfolio
This repository is dedicated to the final code for my latest, example portfolio landing page


<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Liam Martinez</title>
    <link rel="stylesheet" href="./index.css">
    <script src="https://kit.fontawesome.com/c8e4d183c2.js" crossorigin="anonymous"></script>
    <script src="index.js"></script>
    <script type="text/javascript"
        src="https://cdn.jsdelivr.net/npm/@emailjs/browser@3/dist/email.min.js">
</script>
<script type="text/javascript">
   (function(){
      emailjs.init("gPhA_rNvgQpKDMatw");
   })();
</script>
</head>

<body>
    <section id="landing-page" onmousemove="moveBackground(event)">
        <nav>
            <figure>
                <img id="personal-logo" src="./logo.svg" alt="">
            </figure>
            <ul class="nav__link--list">
                <li class="nav__link">
                    <a href="#" class="
                    nav__link--anchor
                    link__hover-effect
                    link__hover-effect--black
                    "onclick="toggleModal()">About</a>
                </li>
                <li class="nav__link">
                    <a href="#projects" class="
                    nav__link--anchor
                    link__hover-effect
                    link__hover-effect--black
                    ">Projects</a>
                </li>
                <li class="nav__link">
                    <a href="#" class="
                    nav__link--anchor
                    link__hover-effect
                    link__hover-effect--black
                    ">Contact</a>
                </li>
                <li class="nav__link click">
                    <a href="#" class="
                    nav__link--anchor
                    link__hover-effect
                    link__hover-effect--black
                    "><i class="fas fa-adjust" onclick="toggleContrast()"></i></a>
                </li>
            </ul>
        </nav>
        <header class="header">
            <div class="header__content">
                <h1 class="title">Hey</h1>
                <h1 class="title orange">I'm Liam</h1>
                <p class="header__para">I am a <b class="orange">Frontend software engineer</b> with a strong passion
                    for building web
                    applications with great user experiences.
                    <br>
                    Here is a bit more <b class="orange click" onclick="toggleModal()">about me.</b>
                </p>
                <div class="social__list">
                    <a href="" class="social__link click">
                        <i class="fab fa-linkedin-in"></i>
                    </a>
                    <a href="https://github.com/Leeyum28" target="_blank" class="social__link click">
                        <i class="fab fa-github"></i>
                    </a>
                    <a href="" class="social__link click">
                        <i class="fas fa-file-pdf"></i>
                    </a>
                </div>
            </div>
        </header>
        <button class="mail__button click" onclick="toggleModal()">
            <i class="fas fa-envelope"></i>
        </button>
        <a href="#projects" class="scroll">
            <div class="scroll__icon click"></div>
        </a>
        <div class="modal">
            <div class="modal__half modal__about">
                <h3 class="modal__title modal__title--about">Here is a bit about me</h3>
                <h4 class="modal__sub-title modal__sub-title--about">Frontend software engineer</h4>
                <p class="modal__para">
                    I'm a 21 year-old <b class="orange">frontend software engineer</b> with an immense passion for creating websites with
                    <b class="orange">tremendous user experiences.</b>
                    <br>
                    Lorem ipsum dolor sit, amet consectetur adipisicing elit. Minima, quasi!
                </p>
                <div class="modal__languages">
                    <figure class="modal__language">
                        <img class="modal__language--img" src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/38/HTML5_Badge.svg/240px-HTML5_Badge.svg.png" alt="">
                        <span class="language__name">HTML</span>
                    </figure>
                    <figure class="modal__language">
                        <img class="modal__language--img" src="https://cdn.iconscout.com/icon/free/png-256/css-131-722685.png" alt="">
                        <span class="language__name">CSS</span>
                    </figure>
                    <figure class="modal__language">
                        <img class="modal__language--img" src="https://cdn.iconscout.com/icon/free/png-256/javascript-1-225993.png" alt="">
                        <span class="language__name">JavaScript</span>
                    </figure>
                </div>
            </div>
            <div class="modal__half modal__contact">
                <i class="fas fa-times modal__exit click" onclick="toggleModal()"></i>
                <h3 class="modal__title modal__title--contact">
                    Let's have a chat!
                </h3>
                <h3 class="modal__sub-title modal__sub-title--contact">
                    I am currently open to new opportunities
                </h3>
                <form id="contact__form" onsubmit="contact(event)">
                    <div class="form__item">
                        <label class="form__item--label">Name</label>
                        <input class="input" name="user_name" type="text" required></input>
                    </div>
                    <div class="form__item">
                        <label class="form__item--label">Email</label>
                        <input class="input" name="user_email" type="email" required></input>
                    </div>
                    <div class="form__item">
                        <label class="form__item--label">Message</label>
                        <textarea class="input" name="message" type="text" required></textarea>
                    </div>
                    <button id="contact__submit" class="form__submit">Send it my way</button>
                </form>
                <div class="modal__overlay modal__overlay--loading">
                    <i class="fas fa-spinner"></i>
                </div>
                <div class="modal__overlay modal__overlay--success">
                    Thanks for the message! Looking forward to speaking with you.
                </div>
            </div>
        </div>
        <img src="./semi circle.svg" class="shape shape--0">
        <img src="./circle.svg" class="shape shape--1">
        <img src="./squiggly.svg" class="shape shape--2">
        <img src="./circle.svg" class="shape shape--3">
        <img src="./triangle.svg" class="shape shape--4">
        <img src="./circle.svg" class="shape shape--5">
        <img src="./squiggly.svg" class="shape shape--6">
        <img src="./circle.svg" class="shape shape--7">
        <img src="./semi circle.svg" class="shape shape--8">
    </section>
    <section id="projects">
        <div class="container">
            <div class="row">
                <h1 class="section__title">
                    Here are some of my <span class="orange">Projects!</span>
                </h1>
                <ul class="project__list">
                    <li class="project">
                        <div class="project__wrapper">
                            <img src="./blinker mockup.png" class="project__img" alt="">
                            <div class="project__wrapper--bg"></div>
                            <div class="project__description">
                                <h3 class="project__description--title">Car Sales Project</h3>
                                <h4 class="project__description--sub-title">HTML, CSS, JavaScript</h4>
                                <p class="project__description--para">
                                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Ea itaque nulla sed,
                                    dolorum eaque quis dolore veritatis omnis dolorem nihil sequi id! A reprehenderit
                                    maiores quos ullam dolore autem facilis.
                                </p>
                                <div class="project__description--links">
                                    <a href="#" class="project__description--link">
                                        <i class="fab fa-github"></i>
                                    </a>
                                    <a href="#" class="project__description--link">
                                        <i class="fas fa-link"></i>
                                    </a>
                                </div>
                            </div>
                        </div>
                    </li>
                </ul>
            </div>
        </div>
    </section>
    <footer>
        <div class="container">
            <div class="row footer__row">
                <figure class="footer__logo--img">
                    <img src="./logo.svg" alt="" class="footer__img">
                </figure>
                <div class="footer__social--list">
                    <a href="#" class="footer__social--link
                    link__hover-effect
                    link__hover-effect--white">
                        Github
                    </a>
                    <a href="#" class="footer__social--link
                    link__hover-effect
                    link__hover-effect--white">
                        Linkedin
                    </a>
                    <a href="#" class="footer__social--link
                    link__hover-effect
                    link__hover-effect--white" onclick="toggleModal()">
                        Contact
                    </a>
                    <a href="#" class="footer__social--link
                    link__hover-effect
                    link__hover-effect--white">
                        Resume
                    </a>
                </div>
                <div class="footer__copyright">Copyright &copy; Liam Martinez</div>
            </div>
        </div>
    </footer>
</body>

</html>


@import url('https://fonts.googleapis.com/css2?family=Lato:wght@400;700&family=Roboto:wght@300;400;500;700;900&display=swap');

* {
    padding: 0;
    margin: 0;
    box-sizing: border-box;
    font-family: 'Roboto', sans-serif;
}




li {
    list-style-type: none;
}

p{
    line-height: 1.5;
    font-size: 16px;
}

html{
    scroll-behavior: smooth;
}


section{
    background-color: rgb(245, 245, 245);
    transition: all 300ms ease;
}

.container{
    padding: 50px 0;
    width: 100%;
}

.row{
    width: 100%;
    max-width: 1100px;
    margin: 0 auto;
    padding: 0 12px;
}


a{
    text-decoration: none;
}

.click{
    cursor: pointer;
    transition: all 300ms ease;
}

.click:hover{
    transform: scale(1.1);
}

.click:active{
    transform: scale(0.9);
}

button{
    cursor: pointer;
}

.link__hover-effect{
    position: relative;
}


.link__hover-effect:after{
    content: '';
    position: absolute;
    bottom: -3px;
    height: 3px;
    width: 0%;
    right: 0;
    background-color: black;
    transition: all 300ms ease;
}

.link__hover-effect--black:after{
    background-color: black;
}
.link__hover-effect--white:after{
    background-color: white;
}

.link__hover-effect:hover:after{
    left: 0;
    width: 100%;
}

input, textarea{
    width: 100%;
    background-color: #242424;
    color: white;
    outline: none;
    border: 2px solid #c0c4cc;
    border-top: none;
    border-left: none;
    border-right: none;
    height: 40px;
    transition: all 600ms ease;
}

textarea{
    resize: vertical;
    height: 100px;
    margin-top: 8px;
}

input:hover, textarea:hover{
    border-color: #dcdfe6;
}

input:focus, textarea:focus{
    border-color: #f06449;
}

label{
    font-size: 14px;
    font-weight: bold;
}

nav,
.scroll,
header{
    opacity: 1;
    visibility: visible;
    transition: all 600ms 800ms;
}


.modal--open nav,
.modal--open .scroll,
.modal--open header{
    opacity: 0;
    visibility: hidden;
    transition: all 400ms;
}

.dark-theme .title,
.dark-theme .section__title,
.dark-theme .section__sub-title,
.dark-theme .nav__link--anchor,
.dark-theme .fa-adjust,
.dark-theme .header__para{
    color: white;
}

.dark-theme section{
    background-color: #242424;
}

.dark-theme #personal-logo{
    filter: none;
}

.dark-theme .scroll__icon{
    border-color: white;
}
.dark-theme .scroll__icon:after,
.dark-theme .link__hover-effect--black:after{
    background-color: white;
}



.dark-theme .mail__button{
    background-color: white;
    color: #242424;
}

/* 

LANDING PAGE

*/


#landing-page{
    min-height: 100vh;
}


header{
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 100%;
    max-width: 1000px;
    padding: 0 30px;
}

.header__para{
    font-size: 24px;
    line-height: 2;
    max-width: 450px;
}

.social__list{
    margin-top: 16px;
    display: flex;
}

.social__link{
    background-color: #f06449;
    color: white;
    padding: 8px 6px;
    width: 32px;
    margin-right: 12px;
    font-size: 14px;
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 75px;
}

.title{
    font-size: 90px;
    margin-bottom: 12px;
    text-align: left;
    line-height: 1;
}
 
.orange {
    color: #f06449;
}


.mail__button{
    width: 70px;
    height: 70px;
    font-size: 32px;
    border-radius: 50px;
    border: none;
    background-color: #242424;
    color: white;
    position: fixed;
    bottom: 32px;
    right: 40px;
    z-index: 1000;
    box-shadow: 0 12px 30px 0 rgb(0, 0, 0, 0.28);
}

.scroll{
    position: absolute;
    bottom: 20px;
    left: 50%;
    transform: translateX(-50%);
}

.scroll__icon{
    width: 20px;
    height: 30px;
    border: 2px solid #242424;
    border-radius: 24px;
    display: flex;
    justify-content: center;
    align-items: center;
}


.scroll__icon:after{
    content: '';
    background-color: #242424;
    width: 4px;
    height: 6px;
    border-radius: 2px;
    animation: scroll 1000ms infinite alternate-reverse;
}


@keyframes scroll{
    0%{
        transform: translateY(3px);
    }
    100%{
        transform: translateY(-3px);
    }
}


/* 

NAVIGATION

*/

#personal-logo{
    height: 50px;
    width: 50px;
    filter: invert(1);
}


nav{
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    max-width: 1200px;
    margin: 0 auto;
    height: 100px;
    padding: 0 20px;
}

.nav__link--list{
    display: flex;
}

.nav__link{
    margin: 0 12px;
}

.nav__link--anchor{
    font-size: 16px;
    color: #242424;
    font-weight: 700;
}

.fa-adjust{
    font-size: 20px;
}


/* 

MODAL

*/

.modal{
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 90%;
    max-width: 1100px;
    min-height: 500px;
    border-radius: 20px;
    overflow: hidden;
    display: flex;
    visibility: hidden;
    transition: visibility 1s, z-index 1s, box-shadow 300ms ease-out;
    z-index: -1;
}


.modal--open .modal{
    z-index: 60;
    visibility: visible;
    box-shadow: 0 20px 80px 0 rgb(0, 0, 0, 0.55);
}



.modal__half{
    width: 50%;
    padding: 40px 72px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    position: relative;
    transition: all 300ms ease-in;
}

.modal--open .modal__about, .modal--open .modal__contact{
    transform: translateX(0%);
}

.modal__about{
    background-color: rgb(245, 245, 245);
    transform: translateX(-110%);
}




.modal__about{
    background-color: rgb(245, 245, 245);
}

.modal__languages{
    display: flex;
    flex-wrap: wrap;
    padding: 16px;
}

.modal__language{
    width: calc(100% / 3);
    position: relative;
    display: flex;
    flex-direction: column;
    align-items: center;
    transition: all 300ms ease;
}
.modal__language:hover .language__name{
    transform: scale(1);
}


.modal__language:hover{
    filter: brightness(80%);
    transform: scale(0.9);
}

.language__name{
    position: absolute;
    bottom: -18px;
    transform: scale(0);
    transition: all 300ms ease;
}


.modal__language--img{
    width: 75%;
    height: 90%;
}

.modal__contact{
    background-color: #242424;
    color: white;
    transform: translateX(110%);
}

.modal__title{
    font-size: 26px;
}
.modal__sub-title{
    margin: 12px 0 24px 0;
    font-size: 14px;
}
.modal__para{
    margin-bottom: 12px;
    line-height: 1.75;
}

.form__item{
    margin-bottom: 20px;
}

.form__submit{
    background-color: #f06449;
    border: 2px solid #f06449;
    color: white;
    font-weight: bold;
    width: 100%;
    max-width: 240px;
    padding: 12px 24px;
    font-size: 20px;
    transition: all 300ms ease;
}


.form__submit:hover{
    border-color: white;
    background-color: transparent;
}
.form__submit:active{
    border-color: #f06449;
    color: #f06449;
}

.modal__overlay{
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    display: none;
    align-items: center;
    justify-content: center;
    z-index: -1;
}

.modal__overlay--loading{
    background-color: #242424;
    font-size: 80px;
}

.modal__overlay--success{
    background-color: #4bb543;
    font-size: 40px;
    font-weight: 700;
    text-align: center;
    padding: 28px;
}

.modal__overlay--visible{
    z-index: 1;
    display: flex;
}



.fa-spinner{
    animation: spinner 750ms infinite;
}

@keyframes spinner{
    0% {
        transform: rotate(0);
    }
    100%{
        transform: rotate(360deg);
    }
}

.modal__exit{
    position: absolute;
    top: 30px;
    right: 40px;
    color: white;
    font-size: 36px;
    z-index: 100;
}


/* 

PROJECTS

*/


.section__title{
    text-align: center;
    margin-bottom: 60px;
    font-size: 48px;
}

.project__img{
    width: 100%;
    transition: all 600ms ease;
}


.project__wrapper{
    position: relative;
    border-radius: 20px;
    box-shadow: 0 20px 80px 0 rgb(0, 0, 0, 0.45);
    overflow: hidden;
}

.project__wrapper:hover .project__description{
    opacity: 1;
    transform: translateY(-50%);
}

.project__wrapper:hover .project__img{
    transform: scale(1.07);
    filter: blur(5px);
    transition: all 600ms ease;
} 

.project__description{
    position: absolute;
    top: 50%;
    left: 90px;
    transform: translateY(100%);
    opacity: 0;
    transition: opacity 300ms, transform 450ms ease;
    color: white;
    max-width: 550px;
}

.project__wrapper:hover .project__wrapper--bg{
    opacity: 0.7;
}


.project__wrapper--bg{
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    opacity: 0;
    background-color: #1c1d25;
    transition: all 450ms ease;
}


.project__description--title{
    font-size: 40px;

}

.project__description--sub-title{
    margin-top: 8px;
}


.project__description--link{
    color: white;
    font-size: 20px;
    margin-right: 16px;
}

.project__description--para{
    margin: 16px 0;
}

/* 

FOOTER

*/



footer{
    position: relative;
    background-color: #242424;
    display: flex;
    padding: 6% 0;
}


.footer__row{
    display: flex;
    flex-direction: column;
    align-items: center;
}

.footer__logo--img{
    width: 70px;
}


.footer__social--list{
    width: 100%;
    max-width: 500px;
    display: flex;
    justify-content: space-around;
    margin: 28px 0;
}

.footer__social--link,
.footer__copyright{
    color: white;
}


.footer__img{
    width: 100%;
}




/* 

SHAPES

*/ 

.shape{
    position: fixed;
}


.shape--0{
    top: 15vh;
    left: 5vw;
}
.shape--1{
    top: 15vh;
    left: 50vw;
}.shape--2{
    top: 15vh;
    left: 80vw;
}.shape--3{
    top: 50vh;
    left: 5vw;
    display: none;
}.shape--4{
    top: 50vh;
    left: 50vw;
}.shape--5{
    top: 50vh;
    left: 80vw;
}.shape--6{
    top: 80vh;
    left: 5vw;
}.shape--7{
    top: 80vh;
    left: 50vw;
}.shape--8{
    top: 80vh;
    left: 80vw;
}




@media (max-width: 768px){
    .title{
        font-size: 80px;
    }
    .header__para{
        font-size: 20px;
    }

    .modal{
        top: 0;
        left: 0;
        height: auto;
        transform: none;
        width: 100%;
        display: flex;
        flex-direction: column-reverse;
        border-radius: 0;
    }
    .modal__half{
        width: 100%;
    }
}


@media (max-width: 480px){
    .title{
        font-size: 52px;

    }
    .header__para{
        font-size: 18px;
    }
    .nav__link:first-child{
        display: none;
    }
    .project__description--para{
        display: none;
    }
    .project__description{
        left: 0;
        padding: 0;
        width: 100%;
        text-align: center;
    }
    .project__description--sub-title{
        margin-bottom: 8px;
    }
    .modal__half{
        padding: 40px;
    }
}
