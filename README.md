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
