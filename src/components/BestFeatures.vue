<template>
    <div>
        <!-- Best Features Start -->
        <section class="best-features-area section-padd4" id="feature">
            <div class="container">
                <div class="row justify-content-end">
                    <div class="col-xl-8 col-lg-10">
                        <!-- Section Tittle -->
                        <div class="row">
                            <div class="col-lg-10 col-md-10">
                                <div class="section-tittle">
                                    <h2 v-html="title"></h2>
                                </div>
                            </div>
                        </div>
                        <!-- Section caption -->
                        <div class="row">
                            
                             <div v-for="feature in bestFeatures" :key="feature.id" class="col-xl-6 col-lg-6 col-md-6">
                                <div class="single-features mb-70">
                                    <div class="features-icon">
                                        <span class="flaticon-support">
                                            <i :class="feature.icon"></i>
                                        </span>
                                    </div>
                                    <div class="features-caption">
                                        <h3>{{ feature.title }}</h3>
                                        <p v-html="feature.desc"></p>
                                    </div>
                                </div>
                            </div>

                        </div>
                    </div>
                </div>
            </div>
            <!-- Shpe -->
            <div class="features-shpae d-none d-lg-block">
                <img :src="featureImg" alt="">
            </div>
        </section>
        <!-- Best Features End -->
    </div>
</template>
<script setup>
    import { ref } from 'vue'
    import {bestFeatures} from '../data/bestFeatures.js'
    const title = ref(`Some of the best features Of Our App!`)
    const featureImg = ref(`../../public//img/shape/best-features.png`)
</script>
<style scoped>
    .best-features-area {
    position: relative;
}
.best-features-area .single-features {
    display: flex;
}
@media (max-width: 767px) {
    .best-features-area .single-features {
    margin-bottom: 30px;
}
}.best-features-area .single-features .features-icon span {
    position: relative;
    color: #fff;
    font-size: 30px;
    height: 67px;
    width: 67px;
    display: block;
    line-height: 67px;
    border-radius: 50%;
    text-align: center;
    background-image: -moz-linear-gradient(90deg,  #e78ae9 0%,  #926ef8 100%);
    background-image: -webkit-linear-gradient(90deg,  #e78ae9 0%,  #926ef8 100%);
    background-image: -ms-linear-gradient(90deg,  #e78ae9 0%,  #926ef8 100%);
}
.best-features-area .single-features .features-caption {
    padding-left: 19px;
}
.best-features-area .single-features .features-caption h3 {
    font-size: 24px;
    font-weight: 600;
    line-height: 1.2;
    margin-bottom: 10px;
    color: #23182c;
}
@media only screen and (min-width: 768px) and (max-width: 991px) {
    .best-features-area .single-features .features-caption p {
    font-size: 15px;
}
}@media only screen and (min-width: 768px) and (max-width: 991px) {
    .best-features-area .single-features .features-caption p {
    font-size: 15px;
}
}@media (max-width: 767px) {
    .best-features-area .single-features .features-caption p {
    font-size: 13px;
}
}.best-features-area .features-shpae {
    position: absolute;
    left: 30px;
    top: 100px;
}
.best-features-area .features-shpae.features-shpae2 {
    top: 300px;
}
@media (min-width: 1200px) and (max-width: 1500px) {
    .best-features-area .features-shpae.features-shpae2 {
    top: 246px !important;
    transform: translateY(0);
}
}@media only screen and (min-width: 992px) and (max-width: 1199px) {
    .best-features-area .features-shpae.features-shpae2 {
    top: 300px;
}
}@media only screen and (min-width: 768px) and (max-width: 991px) {
    .best-features-area .features-shpae.features-shpae2 {
    top: 300px;
}
}@media only screen and (min-width: 1200px) and (max-width: 1300px) {
    .best-features-area .features-shpae {
    top: 50%;
    transform: translateY(-50%);
}
}.best-features-area .features-shpae img {
    max-width: 80%}
@media (min-width: 1200px) and (max-width: 1500px) {
    .best-features-area .features-shpae img {
    max-width: 70%}
}@media only screen and (min-width: 1200px) and (max-width: 1300px) {
    .best-features-area .features-shpae img {
    max-width: 50%;
    top: 50%}
}@media only screen and (min-width: 992px) and (max-width: 1199px) {
    .best-features-area .features-shpae img {
    display: none !important;
}
}
</style>