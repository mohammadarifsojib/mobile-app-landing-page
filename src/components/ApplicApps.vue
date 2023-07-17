<template>
    <div>
        <!-- Applic App Start -->
        <div class="applic-apps section-padding2" id="services">
            <div class="container-fluid">
                <div class="row">
                    <!-- slider Heading -->
                    <div class="col-xl-4 col-lg-4 col-md-8">
                        <div class="single-cases-info mb-30">
                            <h3 v-html="title"></h3>
                            <p v-html="desc"></p>
                        </div>
                    </div>
                    <!-- OwL -->
                    <div class="col-xl-8 col-lg-8 col-md-col-md-7">
                        <div class="app-active d-flex justify-content-end"> 

                            <div v-for="(img, index) in applicApps" :key="index" class="single-cases-img">
                                <img :src="img" alt="">
                            </div>
                            
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <!-- Applic App End -->
    </div>
</template>
<script setup>
    import { applicApps } from '../data/ApplicApps';
    import { ref } from 'vue';
    const title = `Applic Apps<br> Screenshot`
    const desc = `Lorem ipsum dolor sit amet, consecadipiscing elit, sed do eiusmod tempor incididunt ut ore et dolore magna aliqua. Quis ipsum suspendisse gravida. Risus commodo viverra maecenasan lacus vel facilisis.`
</script>
<style scoped>
    .applic-apps {
    overflow: hidden;
    position: relative;
    z-index: 0;
}
.applic-apps .single-cases-info {
    position: relative;
    left: 58%;
    margin-top: 72px;
}
@media only screen and (min-width: 1200px) and (max-width: 1600px) {
    .applic-apps .single-cases-info {
    margin-top: 72px;
    left: 33%}
}@media only screen and (min-width: 992px) and (max-width: 1199px) {
    .applic-apps .single-cases-info {
    left: 38%;
    margin-top: 0px;
}
}@media only screen and (min-width: 768px) and (max-width: 991px) {
    .applic-apps .single-cases-info {
    left: 17%;
    margin-top: 40px;
}
}@media only screen and (min-width: 576px) and (max-width: 767px) {
    .applic-apps .single-cases-info {
    left: 1%;
    margin-top: 20px;
}
}@media (max-width: 767px) {
    .applic-apps .single-cases-info {
    left: 1%;
    margin-top: 10px;
}
}.applic-apps .single-cases-info h3 {
    color: #2b044d;
    font-size: 40px;
    font-weight: 700;
    line-height: 1.3;
    margin-bottom: 20px;
    padding-right: 30px;
}
@media (max-width: 767px) {
    .applic-apps .single-cases-info h3 {
    font-size: 30px;
}
}.applic-apps .single-cases-info p {
    margin-bottom: 50px;
    padding-right: 224px;
}
@media only screen and (min-width: 1200px) and (max-width: 1600px) {
    .applic-apps .single-cases-info p {
    padding-right: 0px;
}
}
@media only screen and (min-width: 992px) and (max-width: 1199px) {
    .applic-apps .single-cases-info p {
    margin-bottom: 20px;
    padding-right: 26px;
}
}
@media only screen and (min-width: 768px) and (max-width: 991px) {
    .applic-apps .single-cases-info p {
    margin-bottom: 20px;
    padding-right: 26px;
}
}
@media (max-width: 767px) {
    .applic-apps .single-cases-info p {
    margin-bottom: 20px;
    padding-right: 0px;
}
}
.app-active > div {
    width: 190px;
    margin-right: 15px;
}
.app-active .single-cases-img img{
    width: 100%;
}

</style>