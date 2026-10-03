<!DOCTYPE html>
<html lang="en">

<head>

<meta charset="UTF-8">

<meta name="viewport"
      content="width=device-width, initial-scale=1.0">

<title>Big Shizzy | Official Artist Profile</title>

<meta name="description"
content="Official profile of Big Shizzy (Toluwani) — artist, entertainer and creative professional from Ogun State, Nigeria.">

<style>

/* =========================================================
   RESET
========================================================= */

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    background: #030303;
    color: #ffffff;

    font-family:
        Arial,
        Helvetica,
        sans-serif;

    line-height: 1.7;

    overflow-x: hidden;
}

img {
    max-width: 100%;
}

a {
    -webkit-tap-highlight-color: transparent;
}

:root {

    --black: #030303;
    --dark: #080808;
    --card: #101010;

    --gold: #d4af37;
    --bright-gold: #f4d675;

    --white: #ffffff;
    --gray: #aaaaaa;
    --light-gray: #d0d0d0;

    --border: rgba(212,175,55,0.22);
}


/* =========================================================
   CUSTOM SCROLLBAR
========================================================= */

::-webkit-scrollbar {
    width: 7px;
}

::-webkit-scrollbar-track {
    background: #050505;
}

::-webkit-scrollbar-thumb {
    background: var(--gold);
    border-radius: 10px;
}


/* =========================================================
   GOLD GLOW
========================================================= */

.gold-glow {
    color: var(--gold);

    text-shadow:
        0 0 10px rgba(212,175,55,.35),
        0 0 30px rgba(212,175,55,.12);
}


/* =========================================================
   HEADER
========================================================= */

header {

    position: fixed;

    top: 0;
    left: 0;

    width: 100%;
    height: 70px;

    z-index: 9999;

    background:
        rgba(0,0,0,.88);

    backdrop-filter: blur(18px);

    -webkit-backdrop-filter: blur(18px);

    border-bottom:
        1px solid
        rgba(212,175,55,.18);
}

.nav {

    width: 100%;
    max-width: 1250px;

    height: 100%;

    margin: auto;

    padding: 0 25px;

    display: flex;

    align-items: center;

    justify-content: space-between;
}

.logo {

    color: var(--gold);

    font-size: 22px;

    font-weight: 900;

    letter-spacing: 2px;

    text-decoration: none;
}

.logo span {
    color: white;
}

nav ul {

    display: flex;

    align-items: center;

    gap: 25px;

    list-style: none;
}

nav a {

    color: white;

    text-decoration: none;

    font-size: 12px;

    font-weight: bold;

    transition: .3s;
}

nav a:hover {
    color: var(--gold);
}


/* =========================================================
   HERO
========================================================= */

.hero {

    min-height: 100vh;

    position: relative;

    overflow: hidden;

    display: flex;

    align-items: center;

    padding:
        130px
        25px
        80px;

    background:

        radial-gradient(
            circle at 70% 30%,
            rgba(212,175,55,.16),
            transparent 30%
        ),

        radial-gradient(
            circle at 10% 80%,
            rgba(212,175,55,.07),
            transparent 30%
        ),

        linear-gradient(
            135deg,
            #030303,
            #0d0d0d
        );
}


/* animated light */

.hero::before {

    content: "";

    position: absolute;

    width: 450px;
    height: 450px;

    border-radius: 50%;

    border:
        1px solid
        rgba(212,175,55,.12);

    right: -150px;
    top: 100px;

    animation:
        rotateGlow 15s linear infinite;
}

@keyframes rotateGlow {

    from {
        transform: rotate(0deg);
    }

    to {
        transform: rotate(360deg);
    }

}


/* =========================================================
   PARTICLES
========================================================= */

.particle {

    position: absolute;

    width: 3px;
    height: 3px;

    background: var(--gold);

    border-radius: 50%;

    opacity: .5;

    box-shadow:
        0 0 10px
        rgba(212,175,55,.8);

    animation:
        floatParticle
        linear
        infinite;
}

.p1 {
    left: 10%;
    top: 25%;
    animation-duration: 8s;
}

.p2 {
    left: 25%;
    top: 70%;
    animation-duration: 11s;
}

.p3 {
    left: 60%;
    top: 20%;
    animation-duration: 9s;
}

.p4 {
    left: 80%;
    top: 65%;
    animation-duration: 13s;
}

.p5 {
    left: 90%;
    top: 30%;
    animation-duration: 10s;
}

@keyframes floatParticle {

    0% {
        transform:
            translateY(0)
            scale(1);

        opacity: .2;
    }

    50% {
        opacity: .8;
    }

    100% {

        transform:
            translateY(-150px)
            scale(.4);

        opacity: 0;
    }

}


/* =========================================================
   HERO CONTAINER
========================================================= */

.hero-container {

    width: 100%;
    max-width: 1200px;

    margin: auto;

    display: grid;

    grid-template-columns:
        1.05fr
        .95fr;

    gap: 70px;

    align-items: center;

    position: relative;

    z-index: 2;
}


/* =========================================================
   HERO TEXT
========================================================= */

.eyebrow {

    color: var(--gold);

    font-size: 13px;

    font-weight: bold;

    letter-spacing: 4px;

    text-transform: uppercase;

    margin-bottom: 20px;
}

.hero-title {

    font-size:
        clamp(
            65px,
            9vw,
            120px
        );

    line-height: .82;

    letter-spacing: -6px;

    font-weight: 900;
}

.hero-title span {

    color: var(--gold);

    text-shadow:
        0 0 30px
        rgba(212,175,55,.15);
}

.hero-description {

    max-width: 650px;

    color: #b5b5b5;

    font-size: 18px;

    margin-top: 30px;
}

.hero-buttons {

    display: flex;

    flex-wrap: wrap;

    gap: 15px;

    margin-top: 35px;
}

.btn {

    display: inline-flex;

    align-items: center;

    justify-content: center;

    min-height: 50px;

    padding:
        13px
        25px;

    border-radius: 5px;

    text-decoration: none;

    font-weight: bold;

    transition: .3s;
}

.btn-gold {

    background: var(--gold);

    color: #000;

    box-shadow:
        0 0 25px
        rgba(212,175,55,.12);
}

.btn-gold:hover {

    background:
        var(--bright-gold);

    transform:
        translateY(-4px);

    box-shadow:
        0 10px 30px
        rgba(212,175,55,.18);
}

.btn-outline {

    color: var(--gold);

    border:
        1px solid
        var(--gold);
}

.btn-outline:hover {

    background:
        var(--gold);

    color: #000;

    transform:
        translateY(-4px);
}


/* =========================================================
   HERO IMAGE
========================================================= */

.hero-photo-wrap {

    position: relative;

    width: 100%;

    max-width: 480px;

    margin: auto;
}

.hero-photo-wrap::before {

    content: "";

    position: absolute;

    inset: -15px;

    border:
        1px solid
        rgba(212,175,55,.25);

    border-radius: 15px;

    animation:
        pulseBorder
        3s ease-in-out infinite;
}

@keyframes pulseBorder {

    0%,
    100% {
        transform: scale(1);

        opacity: .3;
    }

    50% {
        transform: scale(1.025);

        opacity: .8;
    }

}

.hero-photo {

    width: 100%;

    aspect-ratio: 4 / 5;

    object-fit: cover;

    display: block;

    position: relative;

    border-radius: 12px;

    border:
        2px solid
        rgba(212,175,55,.6);

    box-shadow:

        0 0 50px
        rgba(212,175,55,.13),

        0 30px 80px
        rgba(0,0,0,.8);
}


/* =========================================================
   IMAGE LABEL
========================================================= */

.photo-label {

    position: absolute;

    bottom: 20px;
    left: 20px;
    right: 20px;

    padding:
        15px
        18px;

    border-radius: 7px;

    background:
        rgba(0,0,0,.75);

    backdrop-filter: blur(10px);

    border:
        1px solid
        rgba(212,175,55,.3);
}

.photo-label small {

    display: block;

    color: var(--gold);

    font-size: 10px;

    letter-spacing: 2px;

    text-transform: uppercase;
}

.photo-label strong {

    font-size: 20px;
}


/* =========================================================
   SECTION
========================================================= */

section {

    width: 100%;

    padding:
        110px
        25px;
}

.container {

    width: 100%;

    max-width: 1150px;

    margin: auto;
}

.section-heading {

    text-align: center;

    margin-bottom: 65px;
}

.section-heading small {

    color: var(--gold);

    font-size: 12px;

    font-weight: bold;

    letter-spacing: 4px;

    text-transform: uppercase;
}

.section-heading h2 {

    margin-top: 10px;

    font-size:
        clamp(
            38px,
            5vw,
            62px
        );

    line-height: 1.05;
}

.section-heading p {

    max-width: 700px;

    margin:
        18px
        auto
        0;

    color: var(--gray);
}


/* =========================================================
   BIOGRAPHY
========================================================= */

.biography {

    background:
        #080808;
}

.bio-grid {

    display: grid;

    grid-template-columns:
        .8fr
        1.2fr;

    gap: 65px;

    align-items: center;
}

.bio-image {

    position: relative;
}

.bio-image img {

    width: 100%;

    aspect-ratio: 4 / 5;

    object-fit: cover;

    display: block;

    border-radius: 10px;

    border:
        1px solid
        rgba(212,175,55,.4);
}

.bio-content h3 {

    color: var(--gold);

    font-size: 32px;

    margin-bottom: 20px;
}

.bio-content p {

    color: #c3c3c3;

    margin-bottom: 20px;

    font-size: 16px;
}

.bio-signature {

    margin-top: 30px;

    color: var(--gold);

    font-size: 18px;

    font-weight: bold;

    font-style: italic;
}


/* =========================================================
   PROFILE STRIP
========================================================= */

.profile-strip {

    background:
        linear-gradient(
            90deg,
            #0a0a0a,
            #121212,
            #0a0a0a
        );

    border-top:
        1px solid
        rgba(212,175,55,.1);

    border-bottom:
        1px solid
        rgba(212,175,55,.1);

    padding:
        40px
        20px;
}

.profile-items {

    max-width: 1100px;

    margin: auto;

    display: grid;

    grid-template-columns:
        repeat(
            4,
            1fr
        );

    gap: 20px;

    text-align: center;
}

.profile-item {

    padding: 15px;

    border-right:
        1px solid
        #252525;
}

.profile-item:last-child {
    border-right: none;
}

.profile-item span {

    display: block;

    color: var(--gold);

    font-size: 11px;

    letter-spacing: 2px;

    text-transform: uppercase;
}

.profile-item strong {

    display: block;

    margin-top: 5px;

    font-size: 16px;
}


/* =========================================================
   TIMELINE
========================================================= */

.timeline-section {

    background: #030303;
}

.timeline {

    max-width: 900px;

    margin: auto;

    position: relative;
}

.timeline::before {

    content: "";

    position: absolute;

    left: 50%;

    top: 0;
    bottom: 0;

    width: 1px;

    background:
        linear-gradient(
            to bottom,
            transparent,
            var(--gold),
            transparent
        );
}

.timeline-item {

    width: 50%;

    padding:
        0
        40px
        55px;

    position: relative;
}

.timeline-item:nth-child(even) {

    margin-left: 50%;

    padding:
        0
        0
        55px
        40px;
}

.timeline-dot {

    position: absolute;

    top: 5px;

    width: 13px;
    height: 13px;

    border-radius: 50%;

    background: var(--gold);

    box-shadow:
        0 0 15px
        rgba(212,175,55,.7);
}

.timeline-item:nth-child(odd)
.timeline-dot {

    right: -7px;
}

.timeline-item:nth-child(even)
.timeline-dot {

    left: -6px;
}

.timeline-year {

    color: var(--gold);

    font-weight: bold;

    font-size: 13px;

    letter-spacing: 2px;

    margin-bottom: 8px;
}

.timeline-card {

    background: #101010;

    border:
        1px solid
        #222;

    border-radius: 8px;

    padding: 25px;

    transition: .3s;
}

.timeline-card:hover {

    border-color:
        rgba(212,175,55,.6);

    transform:
        translateY(-5px);

    box-shadow:
        0 15px 35px
        rgba(212,175,55,.07);
}

.timeline-card h3 {

    margin-bottom: 8px;
}

.timeline-card p {

    color: var(--gray);

    font-size: 14px;
}


/* =========================================================
   ACHIEVEMENTS
========================================================= */

.achievements {

    background: #090909;
}

.achievement-grid {

    display: grid;

    grid-template-columns:
        repeat(
            3,
            minmax(0,1fr)
        );

    gap: 20px;
}

.achievement-card {

    background:
        linear-gradient(
            145deg,
            #131313,
            #0b0b0b
        );

    border:
        1px solid
        #252525;

    border-radius: 9px;

    padding: 35px 25px;

    position: relative;

    overflow: hidden;

    transition: .3s;
}

.achievement-card::before {

    content: "";

    position: absolute;

    width: 100px;
    height: 100px;

    border-radius: 50%;

    background:
        rgba(212,175,55,.08);

    right: -40px;
    top: -40px;
}

.achievement-card:hover {

    transform:
        translateY(-7px);

    border-color:
        rgba(212,175,55,.6);

    box-shadow:
        0 20px 40px
        rgba(212,175,55,.06);
}

.achievement-number {

    font-size: 32px;

    color: var(--gold);

    font-weight: 900;
}

.achievement-card h3 {

    margin:
        15px
        0
        10px;
}

.achievement-card p {

    color: var(--gray);

    font-size: 14px;
}


/* =========================================================
   CREATIVE IDENTITY
========================================================= */

.identity {

    background: #030303;
}

.identity-grid {

    display: grid;

    grid-template-columns:
        repeat(
            3,
            minmax(0,1fr)
        );

    gap: 20px;
}

.identity-card {

    min-height: 220px;

    padding: 30px 25px;

    background: #0e0e0e;

    border:
        1px solid
        #222;

    border-radius: 8px;

    transition: .3s;
}

.identity-card:hover {

    border-color:
        var(--gold);

    transform:
        translateY(-7px);
}

.identity-icon {

    font-size: 30px;

    color: var(--gold);

    margin-bottom: 15px;
}

.identity-card h3 {

    margin-bottom: 10px;
}

.identity-card p {

    color: var(--gray);

    font-size: 14px;
}


/* =========================================================
   GALLERY
========================================================= */

.gallery {

    background: #080808;
}

.gallery-grid {

    display: grid;

    grid-template-columns:
        repeat(
            12,
            1fr
        );

    grid-auto-rows: 230px;

    gap: 15px;
}

.gallery-item {

    overflow: hidden;

    border-radius: 8px;

    border:
        1px solid
        #252525;

    position: relative;

    background: #111;
}

.gallery-item:nth-child(1) {
    grid-column: span 7;
    grid-row: span 2;
}

.gallery-item:nth-child(2) {
    grid-column: span 5;
}

.gallery-item:nth-child(3) {
    grid-column: span 5;
}

.gallery-item:nth-child(4) {
    grid-column: span 7;
}

.gallery-item:nth-child(5) {
    grid-column: span 5;
}

.gallery-item img {

    width: 100%;
    height: 100%;

    object-fit: cover;

    display: block;

    transition:
        transform .6s;
}

.gallery-item:hover img {

    transform:
        scale(1.08);
}

.gallery-overlay {

    position: absolute;

    left: 0;
    right: 0;
    bottom: 0;

    padding: 25px 18px 18px;

    background:
        linear-gradient(
            transparent,
            rgba(0,0,0,.9)
        );

    transform:
        translateY(100%);

    transition: .3s;
}

.gallery-item:hover
.gallery-overlay {

    transform:
        translateY(0);
}

.gallery-overlay span {

    color: var(--gold);

    font-size: 12px;

    font-weight: bold;
}


/* =========================================================
   SOCIAL
========================================================= */

.social-section {

    text-align: center;

    background:

        radial-gradient(
            circle at center,
            rgba(212,175,55,.12),
            transparent 55%
        ),

        #030303;
}

.social-buttons {

    display: flex;

    justify-content: center;

    flex-wrap: wrap;

    gap: 12px;

    margin-top: 35px;
}

.social-btn {

    min-width: 130px;

    padding:
        13px
        20px;

    border:
        1px solid
        #333;

    border-radius: 5px;

    color: white;

    text-decoration: none;

    font-weight: bold;

    background:
        rgba(255,255,255,.03);

    transition: .3s;
}

.social-btn:hover {

    color: #000;

    background: var(--gold);

    border-color:
        var(--gold);

    transform:
        translateY(-4px);
}

.social-btn.gold {

    background: var(--gold);

    color: #000;

    border-color:
        var(--gold);
}


/* =========================================================
   CTA
========================================================= */

.cta {

    background: #090909;

    text-align: center;
}

.cta-box {

    max-width: 900px;

    margin: auto;

    padding:
        70px
        30px;

    border:
        1px solid
        rgba(212,175,55,.3);

    border-radius: 12px;

    background:
        linear-gradient(
            135deg,
            rgba(212,175,55,.06),
            rgba(255,255,255,.015)
        );
}

.cta-box h2 {

    font-size:
        clamp(
            38px,
            6vw,
            65px
        );

    line-height: 1;

    margin-bottom: 20px;
}

.cta-box p {

    max-width: 650px;

    margin:
        0
        auto
        30px;

    color: var(--gray);
}


/* =========================================================
   FOOTER
========================================================= */

footer {

    background: #000;

    border-top:
        1px solid
        #1c1c1c;

    padding:
        35px
        20px;

    text-align: center;
}

.footer-logo {

    color: var(--gold);

    font-size: 22px;

    font-weight: 900;

    letter-spacing: 2px;
}

footer p {

    color: #666;

    font-size: 13px;

    margin-top: 7px;
}


/* =========================================================
   BACK TO TOP
========================================================= */

.back-top {

    position: fixed;

    right: 20px;
    bottom: 20px;

    width: 45px;
    height: 45px;

    display: flex;

    align-items: center;
    justify-content: center;

    background: var(--gold);

    color: #000;

    border-radius: 50%;

    text-decoration: none;

    font-size: 20px;

    font-weight: bold;

    opacity: 0;

    pointer-events: none;

    transition: .3s;

    z-index: 5000;
}

.back-top.show {

    opacity: 1;

    pointer-events: auto;
}


/* =========================================================
   SCROLL ANIMATION
========================================================= */

.reveal {

    opacity: 0;

    transform:
        translateY(35px);

    transition:
        opacity .8s ease,
        transform .8s ease;
}

.reveal.active {

    opacity: 1;

    transform:
        translateY(0);
}


/* =========================================================
   TABLET
========================================================= */

@media (max-width: 900px) {

    .hero-container {

        grid-template-columns: 1fr;

        text-align: center;

        gap: 55px;
    }

    .hero-description {

        margin-left: auto;
        margin-right: auto;
    }

    .hero-buttons {

        justify-content: center;
    }

    .hero-photo-wrap {

        width:
            min(
                400px,
                85vw
            );
    }

    .bio-grid {

        grid-template-columns: 1fr;

        gap: 45px;
    }

    .bio-image {

        max-width: 500px;

        margin: auto;
    }

    .achievement-grid {

        grid-template-columns:
            repeat(
                2,
                1fr
            );
    }

    .identity-grid {

        grid-template-columns:
            repeat(
                2,
                1fr
            );
    }

    .profile-items {

        grid-template-columns:
            repeat(
                2,
                1fr
            );
    }

    .profile-item:nth-child(2) {

        border-right: none;
    }

}


/* =========================================================
   MOBILE
========================================================= */

@media (max-width: 600px) {

    header {
        height: 64px;
    }

    .nav {
        padding: 0 14px;
    }

    .logo {
        font-size: 16px;
    }

    nav ul {
        gap: 8px;
    }

    nav a {
        font-size: 8px;
    }

    .hero {

        min-height: auto;

        padding:
            115px
            16px
            80px;
    }

    section {

        padding:
            80px
            16px;
    }

    .hero-title {

        font-size:
            clamp(
                58px,
                17vw,
                80px
            );

        letter-spacing:
            -4px;
    }

    .hero-description {

        font-size: 15px;
    }

    .hero-buttons {

        flex-direction: column;

        align-items: stretch;
    }

    .btn {

        width: 100%;
    }

    .hero-photo-wrap {

        width:
            min(
                320px,
                86vw
            );
    }

    .photo-label strong {
        font-size: 17px;
    }

    .profile-items {

        grid-template-columns: 1fr;
    }

    .profile-item {

        border-right: none;

        border-bottom:
            1px solid
            #252525;

        padding-bottom: 20px;
    }

    .profile-item:last-child {
        border-bottom: none;
    }

    .timeline::before {

        left: 8px;
    }

    .timeline-item,
    .timeline-item:nth-child(even) {

        width: 100%;

        margin-left: 0;

        padding:
            0
            0
            35px
            35px;
    }

    .timeline-item:nth-child(odd)
    .timeline-dot,
    .timeline-item:nth-child(even)
    .timeline-dot {

        left: 2px;
        right: auto;
    }

    .achievement-grid {

        grid-template-columns: 1fr;
    }

    .identity-grid {

        grid-template-columns: 1fr;
    }

    .gallery-grid {

        grid-template-columns: 1fr;

        grid-auto-rows:
            260px;
    }

    .gallery-item:nth-child(1),
    .gallery-item:nth-child(2),
    .gallery-item:nth-child(3),
    .gallery-item:nth-child(4),
    .gallery-item:nth-child(5) {

        grid-column: span 1;

        grid-row: span 1;
    }

    .gallery-overlay {

        transform:
            translateY(0);
    }

    .cta-box {

        padding:
            50px
            20px;
    }

}


/* =========================================================
   VERY SMALL PHONES
========================================================= */

@media (max-width: 380px) {

    nav ul {
        gap: 5px;
    }

    nav a {
        font-size: 7px;
    }

    .logo {
        font-size: 14px;
    }

}

</style>

</head>


<body id="top">


<!-- ======================================================
     HEADER
====================================================== -->

<header>

<div class="nav">

    <a
        href="index.html"
        class="logo">

        BIG <span>SHIZZY</span>

    </a>


    <nav>

        <ul>

            <li>
                <a href="index.html">
                    Home
                </a>
            </li>

            <li>
                <a href="#biography">
                    Biography
                </a>
            </li>

            <li>
                <a href="#journey">
                    Journey
                </a>
            </li>

            <li>
                <a href="#gallery">
                    Gallery
                </a>
            </li>

        </ul>

    </nav>

</div>

</header>


<!-- ======================================================
     GOLD PARTICLES
====================================================== -->

<div class="particle p1"></div>
<div class="particle p2"></div>
<div class="particle p3"></div>
<div class="particle p4"></div>
<div class="particle p5"></div>


<!-- ======================================================
     HERO
====================================================== -->

<section class="hero">

<div class="hero-container">


    <div class="reveal">

        <div class="eyebrow">

            Official Artist Profile

        </div>


        <h1 class="hero-title">

            BIG<br>

            <span>SHIZZY</span>

        </h1>


        <p class="hero-description">

            Artist. Entertainer. Creative.

            <br><br>

            Big Shizzy, also known as Toluwani,
            is a creative personality from Ogun State,
            Nigeria, with interests spanning music,
            entertainment, barbing and painting.

        </p>


        <div class="hero-buttons">

            <a
                href="https://wa.me/2349070804147"
                target="_blank"
                rel="noopener"
                class="btn btn-gold">

                Book Big Shizzy

            </a>


            <a
                href="#biography"
                class="btn btn-outline">

                Discover His Story

            </a>

        </div>

    </div>


    <div class="hero-photo-wrap reveal">

        <img
            src="E94E2B62-8DA5-4B74-B19C-E97D8F87F49C.jpeg"
            alt="Big Shizzy"
            class="hero-photo">


        <div class="photo-label">

            <small>
                Artist • Entertainer • Creative
            </small>

            <strong>
                Big Shizzy
            </strong>

        </div>

    </div>


</div>

</section>


<!-- ======================================================
     PROFILE STRIP
====================================================== -->

<div class="profile-strip">

<div class="profile-items">


    <div class="profile-item reveal">

        <span>
            Name
        </span>

        <strong>
            Toluwani
        </strong>

    </div>


    <div class="profile-item reveal">

        <span>
            Stage Name
        </span>

        <strong>
            Big Shizzy
        </strong>

    </div>


    <div class="profile-item reveal">

        <span>
            Origin
        </span>

        <strong>
            Ogun State, Nigeria
        </strong>

    </div>


    <div class="profile-item reveal">

        <span>
            Born
        </span>

        <strong>
            March 22
        </strong>

    </div>


</div>

</div>


<!-- ======================================================
     BIOGRAPHY
====================================================== -->

<section
    class="biography"
    id="biography">

<div class="container">


    <div class="section-heading reveal">

        <small>
            The Story
        </small>

        <h2>
            The Man Behind
            <span class="gold-glow">
                Big Shizzy
            </span>
        </h2>

        <p>
            A creative identity built around entertainment,
            expression, style and ambition.
        </p>

    </div>


    <div class="bio-grid">


        <div class="bio-image reveal">

            <img
                src="E94E2B62-8DA5-4B74-B19C-E97D8F87F49C.jpeg"
                alt="Big Shizzy portrait">

        </div>


        <div class="bio-content reveal">

            <h3>
                Big Shizzy (Toluwani)
            </h3>


            <p>

                Big Shizzy is an artist and entertainer
                from Ogun State, Nigeria. His creative
                identity brings together a passion for
                entertainment, music, personal style and
                artistic expression.

            </p>


            <p>

                His interests extend beyond music.
                Barbing and painting provide additional
                creative outlets, giving him different
                ways to express ideas, personality and
                visual creativity.

            </p>


            <p>

                Through artist promotion, branding,
                entertainment and media services,
                Big Shizzy is developing a platform
                designed to connect artists, brands,
                audiences and creative projects.

            </p>


            <p>

                The Big Shizzy identity represents a
                continuing journey of creativity —
                building a recognizable name while
                creating opportunities within the
                entertainment and creative space.

            </p>


            <div class="bio-signature">

                — Big Shizzy

            </div>

        </div>


    </div>

</div>

</section>


<!-- ======================================================
     JOURNEY
====================================================== -->

<section
    class="timeline-section"
    id="journey">

<div class="container">


    <div class="section-heading reveal">

        <small>
            Creative Journey
        </small>

        <h2>
            The Journey
        </h2>

        <p>
            Key areas of development behind the Big Shizzy identity.
        </p>

    </div>


    <div class="timeline">


        <div class="timeline-item reveal">

            <div class="timeline-dot"></div>

            <div class="timeline-year">
                THE BEGINNING
            </div>

            <div class="timeline-card">

                <h3>
                    Discovering Creativity
                </h3>

                <p>

                    The Big Shizzy identity grows from
                    an interest in entertainment,
                    creativity and self-expression.

                </p>

            </div>

        </div>


        <div class="timeline-item reveal">

            <div class="timeline-dot"></div>

            <div class="timeline-year">
                CREATIVE DEVELOPMENT
            </div>

            <div class="timeline-card">

                <h3>
                    Expanding Creative Skills
                </h3>

                <p>

                    Music, barbing and painting become
                    different channels through which
                    creativity and personality can be
                    expressed.

                </p>

            </div>

        </div>


        <div class="timeline-item reveal">

            <div class="timeline-dot"></div>

            <div class="timeline-year">
                BRAND BUILDING
            </div>

            <div class="timeline-card">

                <h3>
                    Building Big Shizzy
                </h3>

                <p>

                    The creative identity develops into
                    a recognizable personal brand focused
                    on entertainment and creative work.

                </p>

            </div>

        </div>


        <div class="timeline-item reveal">

            <div class="timeline-dot"></div>

            <div class="timeline-year">
                CURRENT FOCUS
            </div>

            <div class="timeline-card">

                <h3>
                    Entertainment & Media
                </h3>

                <p>

                    Current activities include artist
                    promotion, branding, entertainment,
                    media opportunities and creative
                    collaborations.

                </p>

            </div>

        </div>


        <div class="timeline-item reveal">

            <div class="timeline-dot"></div>

            <div class="timeline-year">
                THE FUTURE
            </div>

            <div class="timeline-card">

                <h3>
                    Growing The Platform
                </h3>

                <p>

                    The vision is to continue developing
                    the Big Shizzy brand and create
                    opportunities across entertainment,
                    media and creative projects.

                </p>

            </div>

        </div>


    </div>

</div>

</section>


<!-- ======================================================
     ACHIEVEMENTS
====================================================== -->

<section class="achievements">

<div class="container">


    <div class="section-heading reveal">

        <small>
            Milestones
        </small>

        <h2>
            What He's Building
        </h2>

        <p>
            The areas that define the continuing growth
            of the Big Shizzy brand.
        </p>

    </div>


    <div class="achievement-grid">


        <div class="achievement-card reveal">

            <div class="achievement-number">
                01
            </div>

            <h3>
                Personal Brand
            </h3>

            <p>

                Establishing Big Shizzy as a recognizable
                creative and entertainment identity.

            </p>

        </div>


        <div class="achievement-card reveal">

            <div class="achievement-number">
                02
            </div>

            <h3>
                Multiple Creative Fields
            </h3>

            <p>

                Combining music, entertainment,
                barbing and painting under one
                creative identity.

            </p>

        </div>


        <div class="achievement-card reveal">

            <div class="achievement-number">
                03
            </div>

            <h3>
                Entertainment Platform
            </h3>

            <p>

                Developing services around artist
                promotion, branding, media and
                entertainment.

            </p>

        </div>


        <div class="achievement-card reveal">

            <div class="achievement-number">
                04
            </div>

            <h3>
                Creative Network
            </h3>

            <p>

                Creating opportunities for connections
                between artists, brands, audiences and
                creative projects.

            </p>

        </div>


        <div class="achievement-card reveal">

            <div class="achievement-number">
                05
            </div>

            <h3>
                Professional Presence
            </h3>

            <p>

                Building a professional online presence
                that represents the Big Shizzy brand.

            </p>

        </div>


        <div class="achievement-card reveal">

            <div class="achievement-number">
                06
            </div>

            <h3>
                Future Growth
            </h3>

            <p>

                Continuing to develop the brand,
                creative work and entertainment
                opportunities.

            </p>

        </div>


    </div>

</div>

</section>


<!-- ======================================================
     CREATIVE IDENTITY
====================================================== -->

<section class="identity">

<div class="container">


    <div class="section-heading reveal">

        <small>
            Creative Identity
        </small>

        <h2>
            More Than One Dimension
        </h2>

        <p>
            Different creative interests. One identity.
        </p>

    </div>


    <div class="identity-grid">


        <div class="identity-card reveal">

            <div class="identity-icon">
                ♪
            </div>

            <h3>
                Music
            </h3>

            <p>

                Music forms an important part of the
                Big Shizzy entertainment identity,
                connecting performance, creativity
                and audience engagement.

            </p>

        </div>


        <div class="identity-card reveal">

            <div class="identity-icon">
                ★
            </div>

            <h3>
                Entertainment
            </h3>

            <p>

                Entertainment, events, promotion and
                media opportunities form a central
                part of the professional direction.

            </p>

        </div>


        <div class="identity-card reveal">

            <div class="identity-icon">
                ✂
            </div>

            <h3>
                Barbing
            </h3>

            <p>

                Barbing represents another expression
                of personal style, grooming and
                creativity.

            </p>

        </div>


        <div class="identity-card reveal">

            <div class="identity-icon">
                ✎
            </div>

            <h3>
                Painting
            </h3>

            <p>

                Painting provides a visual creative
                outlet for ideas, imagination and
                artistic expression.

            </p>

        </div>


        <div class="identity-card reveal">

            <div class="identity-icon">
                ◈
            </div>

            <h3>
                Artist Promotion
            </h3>

            <p>

                Supporting artists with visibility,
                branding, promotion and opportunities
                to connect with audiences.

            </p>

        </div>


        <div class="identity-card reveal">

            <div class="identity-icon">
                ◆
            </div>

            <h3>
                Creative Collaboration
            </h3>

            <p>

                Open to creative projects involving
                entertainment, media, branding and
                artistic collaboration.

            </p>

        </div>


    </div>

</div>

</section>


<!-- ======================================================
     GALLERY
====================================================== -->

<section
    class="gallery"
    id="gallery">

<div class="container">


    <div class="section-heading reveal">

        <small>
            Visual World
        </small>

        <h2>
            Big Shizzy Gallery
        </h2>

        <p>
            A visual presentation of the Big Shizzy brand.
        </p>

    </div>


    <div class="gallery-grid">


        <!-- IMAGE 1 -->

        <div class="gallery-item reveal">

            <img
                src="E94E2B62-8DA5-4B74-B19C-E97D8F87F49C.jpeg"
                alt="Big Shizzy">

            <div class="gallery-overlay">

                <span>
                    BIG SHIZZY
                </span>

            </div>

        </div>


        <!-- IMAGE 2 -->

        <div class="gallery-item reveal">

            <img
                src="01159400-FA46-4488-980C-670B53929D2A.jpeg"
                alt="Big Shizzy entertainment">

            <div class="gallery-overlay">

                <span>
                    ENTERTAINMENT
                </span>

            </div>

        </div>


        <!-- IMAGE 3 -->

        <div class="gallery-item reveal">

            <img
                src="E94E2B62-8DA5-4B74-B19C-E97D8F87F49C.jpeg"
                alt="Big Shizzy creative">

            <div class="gallery-overlay">

                <span>
                    CREATIVE
                </span>

            </div>

        </div>


        <!-- IMAGE 4 -->

        <div class="gallery-item reveal">

            <img
                src="01159400-FA46-4488-980C-670B53929D2A.jpeg"
                alt="Big Shizzy services">

            <div class="gallery-overlay">

                <span>
                    ARTIST PROMOTION
                </span>

            </div>

        </div>


        <!-- IMAGE 5 -->

        <div class="gallery-item reveal">

            <img
                src="E94E2B62-8DA5-4B74-B19C-E97D8F87F49C.jpeg"
                alt="Big Shizzy portrait">

            <div class="gallery-overlay">

                <span>
                    ARTIST • ENTERTAINER
                </span>

            </div>

        </div>


    </div>

</div>

</section>


<!-- ======================================================
     SOCIAL / CONTACT
====================================================== -->

<section class="social-section">

<div class="container">


    <div class="section-heading reveal">

        <small>
            Connect
        </small>

        <h2>
            Follow The Journey
        </h2>

        <p>
            Stay connected with Big Shizzy and future
            entertainment and creative projects.
        </p>

    </div>


    <div class="social-buttons reveal">


        <a
            href="https://wa.me/2349070804147"
            target="_blank"
            rel="noopener"
            class="social-btn gold">

            WhatsApp

        </a>


        <a
            href="mailto:adeshipe94@gmail.com"
            class="social-btn">

            Email

        </a>


        <!--
        ADD SOCIAL LINKS HERE WHEN AVAILABLE.

        Example:

        <a href="YOUR-INSTAGRAM-LINK"
           target="_blank"
           class="social-btn">
            Instagram
        </a>

        <a href="YOUR-TIKTOK-LINK"
           target="_blank"
           class="social-btn">
            TikTok
        </a>

        <a href="YOUR-YOUTUBE-LINK"
           target="_blank"
           class="social-btn">
            YouTube
        </a>
        -->


    </div>

</div>

</section>


<!-- ======================================================
     FINAL CTA
====================================================== -->

<section class="cta">

<div class="container">

    <div class="cta-box reveal">

        <h2>
            Let's Create
            <span class="gold-glow">
                Something Big.
            </span>
        </h2>

        <p>

            For bookings, collaborations, artist promotion,
            branding, entertainment projects and media
            opportunities, connect with Big Shizzy.

        </p>


        <a
            href="https://wa.me/2349070804147?text=Hello%20Big%20Shizzy,%20I%20would%20like%20to%20make%20an%20enquiry."
            target="_blank"
            rel="noopener"
            class="btn btn-gold">

            Contact Big Shizzy

        </a>

    </div>

</div>

</section>


<!-- ======================================================
     FOOTER
====================================================== -->

<footer>

    <div class="footer-logo">
        BIG SHIZZY
    </div>

    <p>
        © <span id="year"></span>
        Big Shizzy. All Rights Reserved.
    </p>

    <p>
        Artist • Entertainer • Creative
    </p>

</footer>


<!-- ======================================================
     BACK TO TOP
====================================================== -->

<a
    href="#top"
    class="back-top"
    id="backTop">

    ↑

</a>


<!-- ======================================================
     JAVASCRIPT
====================================================== -->

<script>

/* =========================================================
   COPYRIGHT YEAR
========================================================= */

document.getElementById("year").textContent =
    new Date().getFullYear();


/* =========================================================
   SCROLL REVEAL
========================================================= */

const revealElements =
    document.querySelectorAll(".reveal");


const revealObserver =
    new IntersectionObserver(

        function(entries) {

            entries.forEach(function(entry) {

                if (entry.isIntersecting) {

                    entry.target.classList.add("active");

                }

            });

        },

        {
            threshold: 0.12
        }

    );


revealElements.forEach(function(element) {

    revealObserver.observe(element);

});


/* =========================================================
   BACK TO TOP BUTTON
========================================================= */

const backTop =
    document.getElementById("backTop");


window.addEventListener(
    "scroll",
    function() {

        if (window.scrollY > 500) {

            backTop.classList.add("show");

        } else {

            backTop.classList.remove("show");

        }

    }
);


/* =========================================================
   IMAGE FALLBACK
========================================================= */

document
    .querySelectorAll("img")
    .forEach(function(image) {

        image.addEventListener(
            "error",
            function() {

                this.style.background =
                    "linear-gradient(135deg,#111,#222)";

                this.style.minHeight =
                    "250px";

                this.style.objectFit =
                    "contain";

            }
        );

    });

</script>


</body>

</html>
