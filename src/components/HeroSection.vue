<template>
    <div>
        <!-- Slider Area Start-->
        <div class="slider-area">
            <div class="slider-active">
                <div class="single-slider slider-height slider-padding sky-blue d-flex align-items-center">
                    <div class="container">
                        <div class="row d-flex align-items-center">
                            <div class="col-lg-6 col-md-9 ">
                                <div class="hero__caption">
                                    <span>{{ smallHeading }}</span>
                                    <h1 v-html="bigHeadding"></h1>
                                    <p v-html="description"></p>
                                    <!-- Slider btn -->
                                   <div class="slider-btns">
                                        <!-- Hero-btn -->
                                        <a :href="heroBtnLink" class="btn radius-btn">{{ heroBtnText }}</a>
                                   </div>
                                </div>
                            </div>
                            <div class="col-lg-6">
                                <div class="hero__img d-none d-lg-block f-right">
                                    <img :src="heroImg" alt="">
                                </div>
                            </div>
                        </div>
                    </div>
                </div> 
            </div>
        </div>
        <!-- Slider Area End -->
    </div>
</template>
<script setup>
    import { ref } from 'vue'
    const smallHeading = ref(`App Landing Page`)
    const bigHeadding = ref(`Get things done<br>with Appco`)
    const description = ref(`Dorem ipsum dolor sitamet, consectetur adipiscing elit, sed do eiusm tempor incididunt ulabore et dolore magna aliqua.`)
    const heroImg = ref(`./img/hero/hero_right.png`)
    const heroBtnText = ref(`Download`)
    const heroBtnLink = ref(`#`)
</script>
<style scoped>
.slider-area {
    margin-top: -1px;
}
.slider-area .hero__caption {
    position: relative;
}
@media (max-width: 767px) {
    .slider-area .hero__caption {
    padding-top: 17px;
}
}.slider-area .hero__caption span {
    display: inline-block;
    color: #2b044d;
    font-size: 16px;
    text-transform: uppercase;
    margin-bottom: 20px;
}
.slider-area .hero__caption h1 {
    font-size: 65px;
    font-weight: 700;
    color: #2b044d;
    font-family: "Nunito", sans-serif;
    line-height: 1.3;
    margin-bottom: 32px;
}
.btn {
  background: #f9218d;
  -moz-user-select: none;
  text-transform: capitalize;
  color: #fff;
  cursor: pointer;
  display: inline-block;
  font-size: 16px;
  font-weight: 400;
  letter-spacing: 1px;
  line-height: 0;
  margin-bottom: 0;
  padding: 30px 44px;
  border-radius: 5px;
  cursor: pointer;
  transition: color 0.4s linear;
  position: relative;
  z-index: 1;
  border: 0;
  overflow: hidden;
  margin: 0;
}
.btn::before {
  content: "";
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background: #da1276;
  z-index: 1;
  border-radius: 5px;
  transition: transform 0.5s;
  transition-timing-function: ease;
  transform-origin: 0 0;
  transition-timing-function: cubic-bezier(0.5,  1.6,  0.4,  0.7);
  transform: scaleX(0);
}
.btn:hover::before {
  transform: scaleX(1);
  color: #fff !important;
  z-index: -1;
}
.btn.focus, .btn:focus {
  outline: 0;
  box-shadow: none;
}
.radius-btn {
  padding: 30px 43px;
  border-radius: 30px;
}
@media only screen and (min-width: 992px) and (max-width: 1199px) {
    .slider-area .hero__caption h1 {
    font-size: 55px;
    line-height: 1.2;
}
}@media only screen and (min-width: 768px) and (max-width: 991px) {
    .slider-area .hero__caption h1 {
    font-size: 50px;
    line-height: 1.2;
}
}@media (max-width: 767px) {
    .slider-area .hero__caption h1 {
    font-size: 29px;
    line-height: 1.4;
}
}.slider-area .hero__caption p {
    margin-bottom: 54px;
    padding-right: 155px;
}
@media only screen and (min-width: 768px) and (max-width: 991px) {
    .slider-area .hero__caption p {
    margin-bottom: 54px;
    padding-right: 0px;
}
}@media (max-width: 767px) {
    .slider-area .hero__caption p {
    margin-bottom: 54px;
    padding-right: 0px;
}
}.slider-area .hero__caption .slider-btns a.video-btn {
    background: #d852e8;
    width: 60px;
    height: 60px;
    display: inline-block;
    text-align: center;
    line-height: 60px;
    border-radius: 50%;
    position: relative;
    margin-left: 16px;
}
.slider-area .hero__caption .slider-btns a.video-btn:hover.ani-btn {
    animation: 1.3s cubic-bezier(0.8,  0,  0,  1) 0s normal none infinite running pulse;
    box-shadow: 0 0 0 0 rgba(61, 1, 68, 0.302);
    -webkit-animation: 1.3s cubic-bezier(217,  70,  233,  1) 0s normal none infinite running pulse;
}
@-webkit-keyframes pulse {
    to {
    box-shadow: 0 0 0 45px rgba(83, 16, 90, 0);
}
}@keyframes pulse {
    to {
    box-shadow: 0 0 0 45px rgba(187, 22, 206, 0);
}
}.slider-area .hero__img img {
    position: relative;
    right: -63px;
}
@media only screen and (min-width: 992px) and (max-width: 1199px) {
    .slider-area .hero__img img {
    right: 0px;
}
}
@media only screen and (min-width: 1200px) and (max-width: 1300px) {
    .slider-area .hero__img img {
    right: 0px;
}
}
.slider-area .hero-cap h2 {
    color: #fff;
    font-size: 50px;
    font-weight: 700;
    text-transform: capitalize;
}
.slider-height2 {
    min-height: 300px;
    background-repeat: no-repeat;
    background-position: center center;
}
@media (max-width: 767px) {
    .slider-height2 {
    min-height: 260px;
}
}
.slider-padding {
    padding-top: 130px;
}
@media (max-width: 767px) {
    .slider-padding {
    padding-top: 40px;
}
}@media only screen and (min-width: 576px) and (max-width: 767px) {
    .slider-padding {
    padding-top: 40px;
}
}@media only screen and (min-width: 768px) and (max-width: 991px) {
    .slider-padding {
    padding-top: 40px;
}
}@media only screen and (min-width: 992px) and (max-width: 1199px) {
    .slider-padding {
    padding-top: 100px;
}
}
.hero-caption span {
    color: #fff;
    font-size: 16px;
    display: block;
    margin-bottom: 24px;
    font-weight: 600;
    padding-left: 95px;
    position: relative;
}
.hero-caption span::before {
    position: absolute;
    content: "";
    width: 75px;
    height: 3px;
    background: #8f1bdc;
    left: 0;
    top: 52%;
    transform: translateY(-50%);
}
.hero-caption h2 {
    color: #fff;
    font-size: 50px;
    font-weight: 700;
}
.slider-height {
    min-height: 1000px;
    background-repeat: no-repeat;
    background-position: center center;
}
@media only screen and (min-width: 1200px) and (max-width: 1600px) {
    .slider-height {
    min-height: 900px;
}
}@media only screen and (min-width: 768px) and (max-width: 991px) {
    .slider-height {
    min-height: 600px;
}
}@media (max-width: 767px) {
    .slider-height {
    min-height: 600px;
}
}
.slider-padding {
    padding-top: 130px;
}
@media (max-width: 767px) {
    .slider-padding {
    padding-top: 40px;
}
}@media only screen and (min-width: 576px) and (max-width: 767px) {
    .slider-padding {
    padding-top: 40px;
}
}@media only screen and (min-width: 768px) and (max-width: 991px) {
    .slider-padding {
    padding-top: 40px;
}
}@media only screen and (min-width: 992px) and (max-width: 1199px) {
    .slider-padding {
    padding-top: 100px;
}
}.slider-area {
    margin-top: -1px;
}
.slider-area .hero__caption {
    position: relative;
}
@media (max-width: 767px) {
    .slider-area .hero__caption {
    padding-top: 17px;
}
}.slider-area .hero__caption span {
    display: inline-block;
    color: #2b044d;
    font-size: 16px;
    text-transform: uppercase;
    margin-bottom: 20px;
}
.slider-area .hero__caption h1 {
    font-size: 65px;
    font-weight: 700;
    color: #2b044d;
    font-family: "Nunito", sans-serif;
    line-height: 1.3;
    margin-bottom: 32px;
}
@media only screen and (min-width: 992px) and (max-width: 1199px) {
    .slider-area .hero__caption h1 {
    font-size: 55px;
    line-height: 1.2;
}
}@media only screen and (min-width: 768px) and (max-width: 991px) {
    .slider-area .hero__caption h1 {
    font-size: 50px;
    line-height: 1.2;
}
}@media (max-width: 767px) {
    .slider-area .hero__caption h1 {
    font-size: 29px;
    line-height: 1.4;
}
}.slider-area .hero__caption p {
    margin-bottom: 54px;
    padding-right: 155px;
}
@media only screen and (min-width: 768px) and (max-width: 991px) {
    .slider-area .hero__caption p {
    margin-bottom: 54px;
    padding-right: 0px;
}
}@media (max-width: 767px) {
    .slider-area .hero__caption p {
    margin-bottom: 54px;
    padding-right: 0px;
}
}.slider-area .hero__caption .slider-btns a.video-btn {
    background: #d852e8;
    width: 60px;
    height: 60px;
    display: inline-block;
    text-align: center;
    line-height: 60px;
    border-radius: 50%;
    position: relative;
    margin-left: 16px;
}
.slider-area .hero__caption .slider-btns a.video-btn:hover.ani-btn {
    animation: 1.3s cubic-bezier(0.8,  0,  0,  1) 0s normal none infinite running pulse;
    box-shadow: 0 0 0 0 rgba(61, 1, 68, 0.302);
    -webkit-animation: 1.3s cubic-bezier(217,  70,  233,  1) 0s normal none infinite running pulse;
}
@-webkit-keyframes pulse {
    to {
    box-shadow: 0 0 0 45px rgba(83, 16, 90, 0);
}
}@keyframes pulse {
    to {
    box-shadow: 0 0 0 45px rgba(187, 22, 206, 0);
}
}.slider-area .hero__img img {
    position: relative;
    right: -63px;
}
@media only screen and (min-width: 992px) and (max-width: 1199px) {
    .slider-area .hero__img img {
    right: 0px;
}
}@media only screen and (min-width: 1200px) and (max-width: 1300px) {
    .slider-area .hero__img img {
    right: 0px;
}
}z .slider-area .hero-cap h2 {
    color: #fff;
    font-size: 50px;
    font-weight: 700;
    text-transform: capitalize;
}
.slider-height2 {
    min-height: 300px;
    background-repeat: no-repeat;
    background-position: center center;
}
@media (max-width: 767px) {
    .slider-height2 {
    min-height: 260px;
}
}
</style>