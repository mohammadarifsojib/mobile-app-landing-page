<template>
    <div>
        <header>
        <!-- Header Start -->
        <div class="header-area header-transparrent ">
                <div class="main-header header-sticky">
                    <div class="container">
                        <div class="row align-items-center">
                            <!-- Logo -->
                            <div class="col-xl-2 col-lg-2 col-md-2">
                                <div class="logo">
                                    <a href="#"><img src="../../public/img/logo/logo.png" alt=""></a>
                                </div>
                            </div>
                            <div class="col-xl-10 col-lg-10 col-md-10">
                                <!-- Main-menu -->
                                <div class="main-menu f-right d-none d-lg-block">
                                    <nav>
                                        <ul id="navigation">    
                                            <li class="active"><a href="#"> Home</a></li>
                                            <li><a href="#feature">Feature</a></li>
                                            <li><a href="#services">Services</a></li>
                                            <li><a href="#pricing">Pricing</a></li>
                                            <li><a href="#">Pages</a>
                                                <ul class="submenu">
                                                    <li><a href="blog.html">Blog</a></li>
                                                    <li><a href="single-blog.html">Blog Details</a></li>
                                                    <li><a href="elements.html">Element</a></li>
                                                </ul>
                                            </li>
                                            <li><a href="#contact">Contact</a></li>
                                        </ul>
                                    </nav>
                                </div>
                            </div>
                            <!-- Mobile Menu -->
                            <div class="col-12">
                                <div class="mobile_menu d-block d-lg-none"></div>
                            </div>
                        </div>
                    </div>
                </div>
        </div>
            <!-- Header End -->
        </header>
    </div>
</template>

<script setup>
    import { onMounted } from 'vue'
    import $ from 'jquery'

    $(window).on('scroll', function () {
      var scroll = $(window).scrollTop();
      if (scroll < 245) {
        $(".header-sticky").removeClass("sticky-bar");
      } else {
        $(".header-sticky").addClass("sticky-bar");
      }
    });

    $(window).on('scroll', function () {
      var scroll = $(window).scrollTop();
      if (scroll < 245) {
          $(".header-sticky").removeClass("sticky");
      } else {
          $(".header-sticky").addClass("sticky");
      }
    });


</script>

<style scoped>
    .header-btn {
        background: #4043bc;
        padding: 20px 11px;
        min-width: 120px;
        position: relative;
    }
    .header-btn::before {
        background: #ec4683;
    }
    .header-transparrent {
    position: absolute;
    top: 0;
    right: 0;
    left: 0;
    z-index: 9;
}
.main-header {
    z-index: 3;
}
@media only screen and (min-width: 768px) and (max-width: 991px) {
    .main-header {
    padding: 11px 0;
}
}@media only screen and (min-width: 576px) and (max-width: 767px) {
    .main-header {
    padding: 11px 0;
}
}@media (max-width: 767px) {
    .main-header {
    padding: 11px 0;
}
}@media only screen and (min-width: 1200px) and (max-width: 1600px) {
    .main-header .main-menu {
    margin-right: 30px;
}
}.main-header .main-menu ul li {
    display: inline-block;
    position: relative;
    z-index: 1;
    margin: 0 5px;
}
.main-header .main-menu ul li>a {
    color: #450b78;
    font-weight: 400;
    padding: 39px 16px;
    font-weight: 400;
    display: block;
    font-size: 16px;
    -webkit-transition: .3s;
    -moz-transition: .3s;
    -o-transition: .3s;
    transition: .3s;
    text-transform: capitalize;
}
@media only screen and (min-width: 992px) and (max-width: 1199px) {
    .main-header .main-menu ul li>a {
    padding: 39px 15px;
}
}.main-header .main-menu ul li>a::before {
    position: absolute;
    content: "";
    left: 0;
    bottom: 20px;
    background: #a60dcf;
    height: 2px;
    width: 0;
    transition: .3s;
}
.main-header .main-menu ul li:hover>a::before {
    width: 100%}
.main-header .main-menu ul li.active>a::before {
    width: 100%}
.main-header .main-menu ul ul.submenu {
    position: absolute;
    width: 170px;
    background: #fff;
    left: 0;
    top: 80%;
    visibility: hidden;
    opacity: 0;
    box-shadow: 0 0 10px 3px rgba(0, 0, 0, 0.05);
    padding: 17px 0;
    -webkit-transition: .3s;
    -moz-transition: .3s;
    -o-transition: .3s;
    transition: .3s;
}
.main-header .main-menu ul ul.submenu>li {
    margin-left: 7px;
    display: block;
}
.main-header .main-menu ul ul.submenu>li>a {
    padding: 6px 10px !important;
    font-size: 14px;
    text-transform: capitalize;
}
.main-header .main-menu ul ul.submenu>li>a::before {
    position: absolute;
    content: "";
    left: -5px;
    background: #a60dcf;
    height: 2px;
    width: 0;
    transition: .3s;
    top: 50%}
.main-header .main-menu ul ul.submenu>li>a:hover {
    padding-left: 15px !important;
}
.main-header .main-menu ul ul.submenu>li>a:hover::before {
    width: 10px;
}
.header-area .header-top .header-info-right .header-social a i {
    -webkit-transition: .4s;
    -moz-transition: .4s;
    -o-transition: .4s;
    transition: .4s;
    transform: rotateY(0deg);
    -webkit-transform: rotateY(0deg);
    -moz-transform: rotateY(0deg);
    -ms-transform: rotateY(0deg);
    -o-transform: rotateY(0deg);
}
.header-area .header-top .header-info-right .header-social a:hover i {
    transform: rotateY(180deg);
    -webkit-transform: rotateY(180deg);
    -moz-transform: rotateY(180deg);
    -ms-transform: rotateY(180deg);
    -o-transform: rotateY(180deg);
}
.main-header ul>li:hover>ul.submenu {
    visibility: visible;
    opacity: 1;
    top: 100%}
.top-bg {
    background: #002d5b;
}
.sticky-bar {
    left: 0;
    margin: auto;
    position: fixed;
    top: 0;
    width: 100%;
    -webkit-box-shadow: 0 10px 15px rgba(25, 25, 25, 0.1);
    box-shadow: 0 10px 15px rgba(25, 25, 25, 0.1);
    z-index: 9999;
    -webkit-animation: 300ms ease-in-out 0s normal none 1 running fadeInDown;
    animation: 300ms ease-in-out 0s normal none 1 running fadeInDown;
    -webkit-box-shadow: 0 10px 15px rgba(25, 25, 25, 0.1);
    background: #fff;
}
.header-sticky ul li a {
    padding: 10px 19px;
    text-decoration: none;
}
.header-sticky.sticky-bar.sticky .main-menu ul>li>a {
    padding: 25px 16px;
}
.header-sticky.sticky-bar.sticky .main-menu ul>li>a::before {
    bottom: 11px;
}
.header-transparrent {
    position: absolute;
    top: 0;
    right: 0;
    left: 0;
    z-index: 9;
}
.main-header {
    z-index: 3;
}
@media only screen and (min-width: 768px) and (max-width: 991px) {
    .main-header {
    padding: 11px 0;
}
}@media only screen and (min-width: 576px) and (max-width: 767px) {
    .main-header {
    padding: 11px 0;
}
}@media (max-width: 767px) {
    .main-header {
    padding: 11px 0;
}
}@media only screen and (min-width: 1200px) and (max-width: 1600px) {
    .main-header .main-menu {
    margin-right: 30px;
}
}.main-header .main-menu ul li {
    display: inline-block;
    position: relative;
    z-index: 1;
    margin: 0 5px;
}
.main-header .main-menu ul li>a {
    color: #450b78;
    font-weight: 400;
    padding: 39px 16px;
    font-weight: 400;
    display: block;
    font-size: 16px;
    -webkit-transition: .3s;
    -moz-transition: .3s;
    -o-transition: .3s;
    transition: .3s;
    text-transform: capitalize;
}
@media only screen and (min-width: 992px) and (max-width: 1199px) {
    .main-header .main-menu ul li>a {
    padding: 39px 15px;
}
}.main-header .main-menu ul li>a::before {
    position: absolute;
    content: "";
    left: 0;
    bottom: 20px;
    background: #a60dcf;
    height: 2px;
    width: 0;
    transition: .3s;
}
.main-header .main-menu ul li:hover>a::before {
    width: 100%}
.main-header .main-menu ul li.active>a::before {
    width: 100%}
.main-header .main-menu ul ul.submenu {
    position: absolute;
    width: 170px;
    background: #fff;
    left: 0;
    top: 80%;
    visibility: hidden;
    opacity: 0;
    box-shadow: 0 0 10px 3px rgba(0, 0, 0, 0.05);
    padding: 17px 0;
    -webkit-transition: .3s;
    -moz-transition: .3s;
    -o-transition: .3s;
    transition: .3s;
}
.main-header .main-menu ul ul.submenu>li {
    margin-left: 7px;
    display: block;
}
.main-header .main-menu ul ul.submenu>li>a {
    padding: 6px 10px !important;
    font-size: 14px;
    text-transform: capitalize;
}
.main-header .main-menu ul ul.submenu>li>a::before {
    position: absolute;
    content: "";
    left: -5px;
    background: #a60dcf;
    height: 2px;
    width: 0;
    transition: .3s;
    top: 50%}
.main-header .main-menu ul ul.submenu>li>a:hover {
    padding-left: 15px !important;
}
.main-header .main-menu ul ul.submenu>li>a:hover::before {
    width: 10px;
}
.header-area .header-top .header-info-right .header-social a i {
    -webkit-transition: .4s;
    -moz-transition: .4s;
    -o-transition: .4s;
    transition: .4s;
    transform: rotateY(0deg);
    -webkit-transform: rotateY(0deg);
    -moz-transform: rotateY(0deg);
    -ms-transform: rotateY(0deg);
    -o-transform: rotateY(0deg);
}
.header-area .header-top .header-info-right .header-social a:hover i {
    transform: rotateY(180deg);
    -webkit-transform: rotateY(180deg);
    -moz-transform: rotateY(180deg);
    -ms-transform: rotateY(180deg);
    -o-transform: rotateY(180deg);
}
.main-header ul>li:hover>ul.submenu {
    visibility: visible;
    opacity: 1;
    top: 100%}
.top-bg {
    background: #002d5b;
}
.header-sticky ul li a {
    padding: 10px 19px;
}
.header-sticky.sticky-bar.sticky .main-menu ul>li>a {
    padding: 25px 16px;
}
.header-sticky.sticky-bar.sticky .main-menu ul>li>a::before {
    bottom: 11px;
}
.slicknav_menu .slicknav_icon-bar {
    background-color: #8f1bdc !important;
}
.slicknav_nav {
    margin-top: 0px;
}
.header-sticky.sticky-bar.sticky .header-btn .get-btn {
    padding: 20px 20px;
}
.header-area .slicknav_btn {
    top: -43px;
}
.slicknav_menu .slicknav_nav a:hover {
    background: transparent;
    color: #8f1bdc;
}
.slicknav_menu {
    background: transparent;
    margin-top: 5px !important;
}
.mobile_menu {
    position: absolute;
    right: 0px;
    width: 100%;
    z-index: 99;
}
</style>