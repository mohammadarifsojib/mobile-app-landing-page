<template >
    <div>
        <!-- Available App  Start-->
        <div class="available-app-area">
            <div class="container">
                <div class="row d-flex justify-content-between">
                    <div class="col-xl-5 col-lg-6">
                        <div class="app-caption">
                            <div class="section-tittle section-tittle3">
                                <h2 v-html="title"></h2>
                                <p v-html="description"></p>
                                <div class="app-btn">
                                    <a href="#" class="app-btn1">
                                        <img :src="iosApp" alt="">
                                    </a>
                                    <a href="#" class="app-btn2"><img :src="androidApp" alt=""></a>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="col-xl-6 col-lg-6">
                        <div class="app-img">
                            <img :src="shape" alt="">
                        </div>
                    </div>
                </div>
            </div>
            <!-- Shape -->
            <div class="app-shape">
                <img :src="shapeTop" alt="" class="app-shape-top heartbeat d-none d-lg-block">
                <img :src="shapeLeft" alt="" class="app-shape-left d-none d-xl-block">
                <!-- <img src="assets/img/shape/app-shape-right.png" alt="" class="app-shape-right bounce-animate "> -->
            </div>
        </div>
        <!-- Available App End-->
    </div>
</template>
<script setup>
    import {ref} from 'vue'
    const title = ref(`Our App Available For Any Device Download now`)
    const description = ref(`Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore fug.`)
    const iosApp = ref(`../../public/img/shape/app_btn1.png`)
    const androidApp = ref(`../../public/img/shape/app_btn2.png`)
    const shape = ref(`../../public/img/shape/available-app.png`)
    const shapeTop = ref(`../../public/img/shape/app-shape-top.png`)
    const shapeLeft = ref(`../../public/img/shape/app-shape-left.png`)
</script>
<style scoped>
.available-app-area {
    background-image: -moz-linear-gradient(0deg,  #6c19f6 0%,  #f9218d 100%);
    background-image: -webkit-linear-gradient(0deg,  #6c19f6 0%,  #f9218d 100%);
    background-image: -ms-linear-gradient(0deg,  #6c19f6 0%,  #f9218d 100%);
}
.available-app-area {
    position: relative;
    padding-top: 220px;
    padding-bottom: 220px;
}
@media only screen and (min-width: 992px) and (max-width: 1199px) {
    .available-app-area {
    padding-top: 150px;
    padding-bottom: 150px;
}
}@media only screen and (min-width: 768px) and (max-width: 991px) {
    .available-app-area {
    padding-top: 100px;
    padding-bottom: 100px;
}
}@media only screen and (min-width: 576px) and (max-width: 767px) {
    .available-app-area {
    padding-top: 100px;
    padding-bottom: 100px;
}
}@media (max-width: 767px) {
    .available-app-area {
    padding-top: 100px;
    padding-bottom: 100px;
}
}.available-app-area .app-caption .section-tittle3 h2 {
    color: #fff;
    margin-bottom: 35px;
    font-weight: 600;
}
.available-app-area .app-caption p {
    color: #fff;
    padding-right: 52px;
    padding-bottom: 26px;
}
.available-app-area .app-caption .app-btn .app-btn1 {
    padding-right: 15px;
}
@media (max-width: 767px) {
    .available-app-area .app-caption .app-btn .app-btn2 {
    display: block;
    padding-top: 10px;
}
}.available-app-area .app-img {
    position: relative;
    right: -88px;
}
@media only screen and (min-width: 1200px) and (max-width: 1440px) {
    .available-app-area .app-img {
    right: 0px;
}
}@media only screen and (min-width: 992px) and (max-width: 1199px) {
    .available-app-area .app-img {
    top: 45px;
    right: 0;
}
}@media only screen and (min-width: 768px) and (max-width: 991px) {
    .available-app-area .app-img {
    top: 45px;
    right: 0;
}
}@media only screen and (min-width: 576px) and (max-width: 767px) {
    .available-app-area .app-img {
    top: 45px;
    right: 0;
}
}@media (max-width: 767px) {
    .available-app-area .app-img {
    top: 45px;
    right: 0;
}
}.available-app-area .app-img img {
    width: 100%}
.available-app-area .app-shape .app-shape-top {
    position: absolute;
    top: 100px;
    left: 125px;
}
.available-app-area .app-shape .app-shape-left {
    position: absolute;
    left: 0;
    bottom: 0;
}
.available-app-area .app-shape .app-shape-right {
    position: absolute;
    right: 252px;
    top: 208px;
}
@media only screen and (min-width: 1200px) and (max-width: 1440px) {
    .available-app-area .app-shape .app-shape-right {
    display: none !important;
}
}@media only screen and (min-width: 992px) and (max-width: 1199px) {
    .available-app-area .app-shape .app-shape-right {
    display: none !important;
}
}@media only screen and (min-width: 768px) and (max-width: 991px) {
    .available-app-area .app-shape .app-shape-right {
    display: none !important;
}
}@media only screen and (min-width: 576px) and (max-width: 767px) {
    .available-app-area .app-shape .app-shape-right {
    display: none !important;
}
}@media (max-width: 767px) {
    .available-app-area .app-shape .app-shape-right {
    display: none !important;
}
}
</style>