<template>
    <div>
        <!-- Best Pricing Start -->
        <section class="best-pricing pricing-padding" style="background-image: url('../../public/img/gallery/best_pricingbg.jpg');z-index:-1" id="pricing">
            <div class="container">
                <!-- Section Tittle -->
                <div class="row d-flex justify-content-center">
                    <div class="col-lg-6 col-md-8">
                        <div class="section-tittle section-tittle2 text-center">
                            <h2 v-html="title"></h2>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        <!-- Best Pricing End -->
        <!-- Pricing Card Start -->
        <div class="pricing-card-area">
            <div class="container">
                <div class="row">
                    
                    <div v-for="price in pricing" :key="price.id" class="col-xl-4 col-lg-4 col-md-6">
                        <div class="single-card  text-center mb-30">
                            <div class="card-top">
                                <span>{{ price.duration }}</span>
                                <h4>
                                    {{ price.priceUnit }}{{ price.price }} <span>/ {{ price.validFor }}</span>
                                </h4>
                            </div>
                            <div class="card-bottom">
                                <ul>
                                    <li v-for="(offer, index) in price.offers" :key="index">
                                        {{ offer }}
                                    </li>
                                </ul>
                                <a :href="price.btnLink" class="btn card-btn1">{{ price.btnText }}</a>
                            </div>
                        </div>
                    </div>

                </div>
            </div>
        </div>
        <!-- Pricing Card End -->
    </div>
</template>
<script setup>
    import { ref } from 'vue';
    import { pricing } from '../data/Pricing.js'
    const title = ref(`Choose Your Very Best Pricing Plan.`)
</script>
<style scoped>
    .best-pricing {
    position: relative;
}
.best-pricing.pricing-padding {
    padding-top: 110px;
    padding-bottom: 280px;
    background-size: cover;
    background-repeat: no-repeat;
}
.best-pricing.pricing-padding2 {
    padding-top: 300px;
    padding-bottom: 280px;
}
@media only screen and (min-width: 992px) and (max-width: 1199px) {
    .best-pricing.pricing-padding2 {
    padding-top: 300px;
    padding-bottom: 280px;
}
}@media only screen and (min-width: 768px) and (max-width: 991px) {
    .best-pricing.pricing-padding2 {
    padding-top: 160px;
}
}@media only screen and (min-width: 576px) and (max-width: 767px) {
    .best-pricing.pricing-padding2 {
    padding-top: 160px;
}
}@media (max-width: 767px) {
    .best-pricing.pricing-padding2 {
    padding-top: 160px;
}
}
.best-pricing::before {
    position: absolute;
    width: 100%;
    height: 100%;
    left: 0;
    right: 0;
    top: 0;
    bottom: 0;
    content: "";
    opacity: 0.95;
    background-image: -moz-linear-gradient(0deg,  #f9218d 0%,  #6c19f6 100%);
    background-image: -webkit-linear-gradient(0deg,  #f9218d 0%,  #6c19f6 100%);
    background-image: -ms-linear-gradient(0deg,  #f9218d 0%,  #6c19f6 100%);
    z-index: 1;
}
.best-pricing.best-pricing2::before {
    display: none;
}
.pricing-card-area {
    margin-top: -295px;
}
.pricing-card-area .single-card {
    position: relative;
    background: #fff;
    padding: 40px 25px;
    border-radius: 6px;
    box-shadow: 0px 0px 9px 0px rgba(131, 93, 248, 0.07);
    -webkit-transition: .4s;
    -moz-transition: .4s;
    -o-transition: .4s;
    transition: .4s;
}
.pricing-card-area .single-card::before {
    background-image: url(../../public/img/gallery/card_dot.png);
    content: "";
    width: 171px;
    height: 134px;
    position: absolute;
    right: 2px;
    bottom: 2px;
    z-index: -1;
    -webkit-transition: .4s;
    -moz-transition: .4s;
    -o-transition: .4s;
    transition: .4s;
}
@media (max-width: 767px) {
    .pricing-card-area .single-card::before {
    display: none;
}
}.pricing-card-area .single-card .card-top {
    border-bottom: 2px solid #f4f4f4;
    margin-bottom: 46px;
}
.pricing-card-area .single-card .card-top span {
    color: #57667e;
    font-size: 24px;
    margin-bottom: 19px;
    display: inline-block;
}
.pricing-card-area .single-card .card-top h4 {
    color: #6a56a6;
    font-size: 50px;
    font-weight: 500;
    margin-bottom: 26px;
    padding-right: 3px;
    font-family: "Poppins", sans-serif;
}
.pricing-card-area .single-card .card-top h4 span {
    color: #6a56a6;
    font-size: 16px;
}
.pricing-card-area .single-card .card-bottom ul li {
    color: #717081;
    font-weight: 300;
    margin-bottom: 16px;
    font-size: 16px;
}
.pricing-card-area .single-card .card-bottom ul li:last-child {
    margin-bottom: 45px;
}
.pricing-card-area .single-card.active {
    box-shadow: 0px 10px 30px 0px rgba(133, 66, 189, 0.1);
}
.pricing-card-area .single-card.active::before {
    right: -20px;
    bottom: -21px;
}
.pricing-card-area .single-card.active .btn::before {
    transform: scaleX(1);
    color: #fff !important;
    z-index: -1;
}
.pricing-card-area .single-card:hover {
    box-shadow: 0px 10px 30px 0px rgba(133, 66, 189, 0.1);
}
.pricing-card-area .single-card:hover::before {
    right: -20px;
    bottom: -21px;
}
.pricing-card-area .single-card:hover .btn::before {
    transform: scaleX(1);
    color: #fff !important;
    z-index: -1;
}

.section-tittle2 h2 {
  color: #fff;
  position: relative;
  z-index: 3;
}
</style>