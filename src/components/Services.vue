<template>
    <div>
        <!-- Services Area Start -->
        <section class="service-area sky-blue section-padding2">
            <div class="container">
                <!-- Section Tittle -->
                <div class="row d-flex justify-content-center">
                    <div class="col-lg-6">
                        <div class="section-tittle text-center">
                            <p v-html="title"></p>
                        </div>
                    </div>
                </div>
                <!-- Section caption -->
                <div class="row">
                    <div v-for="service in services" :key="service.id" class="col-xl-4 col-lg-4 col-md-6">
                        <div class="services-caption text-center mb-30">
                            <div class="service-icon">
                                <span class="flaticon-businessman">
                                    <i :class="service.icon"></i>
                                </span>
                            </div> 
                            <div class="service-cap">
                                <h4><a href="#">{{ service.title }}</a></h4>
                                <p>{{ service.desc }}</p>
                            </div>
                        </div>
                    </div>

                </div>
            </div>
        </section>
        <!-- Services Area End -->
    </div>
</template>
<script setup>
    import {services} from '../data/services.js'
    import {ref} from 'vue'

    const title = `<h2>How Can We HelpYour<br>with Appco!</h2>`
    
</script>
<style scoped>
    .service-area .services-caption {
    background: #fff;
    padding: 84px 45px 56px;
    border: 1px solid transparent;
    border-radius: 7px;
    -webkit-transition: .5s;
    -moz-transition: .5s;
    -o-transition: .5s;
    transition: .5s;
}
@media only screen and (min-width: 992px) and (max-width: 1199px) {
    .service-area .services-caption {
    padding: 84px 25px 56px;
}
}.service-area .services-caption .service-icon {
    display: inline-block;
    position: relative;
}
.service-area .services-caption .service-icon::before {
    background-image: url(../img/shape/dot-bg.png);
    content: "";
    width: 80px;
    height: 135px;
    position: absolute;
    right: -29px;
    top: -35px;
    z-index: 0;
    -webkit-transition: .5s;
    -moz-transition: .5s;
    -o-transition: .5s;
    transition: .5s;
}
.service-area .services-caption .service-icon span {
    position: relative;
    color: #fff;
    font-size: 40px;
    height: 105px;
    width: 105px;
    display: block;
    line-height: 105px;
    border-radius: 50%;
    text-align: center;
    background: #e88cea;
    margin-bottom: 42px;
    -webkit-transition: .5s;
    -moz-transition: .5s;
    -o-transition: .5s;
    transition: .5s;
}
.service-area .services-caption .service-cap h4 a {
    font-size: 24px;
    font-weight: 700;
    line-height: 1.2;
    margin-bottom: 27px;
    display: inline-block;
    text-decoration: none;
}
.service-area .services-caption .service-cap h4 a:hover {
    color: #835ef8;
}
.services-caption:hover {
    border: 1px solid #b8a2ff;
}
.services-caption:hover .service-icon::before {
    right: -32px;
}
.services-caption:hover .service-icon span {
    background: #835ef8;
}
.services-caption.active {
    border: 1px solid #b8a2ff;
}
.services-caption.active .service-icon::before {
    right: -32px;
}
.services-caption.active .service-icon span {
    background: #835ef8;
}
.services-area {
    padding-top: 270px;
}
@media only screen and (min-width: 992px) and (max-width: 1199px) {
    .services-area {
    padding-top: 200px;
}
}@media only screen and (min-width: 768px) and (max-width: 991px) {
    .services-area {
    padding-top: 150px;
}
}@media only screen and (min-width: 576px) and (max-width: 767px) {
    .services-area {
    padding-top: 150px;
}
}@media (max-width: 767px) {
    .services-area {
    padding-top: 130px;
}
}
.section-tittle h2 {
    font-size: 50px;
    font-weight: 700;
    line-height: 1.2;
    margin-bottom: 90px;
}
@media (max-width: 767px) {
    .section-tittle h2 {
    font-size: 30px;
    line-height: 1.3;
}
}@media only screen and (min-width: 992px) and (max-width: 1199px) {
    .section-tittle h2 {
    font-size: 40px;
}
}
</style>