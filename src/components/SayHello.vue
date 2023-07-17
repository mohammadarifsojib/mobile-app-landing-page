<template>
    <div>
        <!-- Say Something Start -->
        <div class="say-something-aera pt-90 pb-90 fix" id="contact">
            <div class="container">
                <div class="row justify-content-between align-items-center">
                    <div class="offset-xl-1 offset-lg-1 col-xl-5 col-lg-5">
                        <div class="say-something-cap">
                            <h2 v-html="title"></h2>
                        </div>
                    </div>
                    <div class="col-xl-2 col-lg-3">
                        <div class="say-btn">
                            <a :href="ctaLink" class="btn radius-btn">{{ ctaText }}</a>
                        </div>
                    </div>
                </div>
            </div>
            <!-- shape -->
            <div class="say-shape">
                <img :src="shapeOne" alt="" class="say-shape1 rotateme d-none d-xl-block">
                <img :src="shapeTwo" alt="" class="say-shape2 d-none d-lg-block">
            </div>
        </div>
        <!-- Say Something End -->
    </div>
</template>
<script setup>
    import { ref } from 'vue'
    const title = ref(`Say Hello To The Collaboration Hub.`)
    const ctaText = ref(`Contact Us`)
    const ctaLink = ref(`#`)
    const shapeOne = ref(`./img/shape/say-shape-left.png`)
    const shapeTwo = ref(`./img/shape/say-shape-right.png`)
</script>
<style scoped>
    .say-something-aera {
    position: relative;
    border-bottom: 1px solid #ffc9fd;
}
.say-something-aera .say-something-cap h2 {
    font-size: 50px;
    font-weight: 700;
    line-height: 1.2;
    color: #282828;
}
@media only screen and (min-width: 992px) and (max-width: 1199px) {
    .say-something-aera .say-something-cap h2 {
    font-size: 41px;
}
}@media only screen and (min-width: 768px) and (max-width: 991px) {
    .say-something-aera .say-something-cap h2 {
    margin-bottom: 25px;
}
}@media only screen and (min-width: 576px) and (max-width: 767px) {
    .say-something-aera .say-something-cap h2 {
    margin-bottom: 25px;
    font-size: 41px;
}
}@media (max-width: 767px) {
    .say-something-aera .say-something-cap h2 {
    margin-bottom: 25px;
    font-size: 30px;
}
}.say-something-aera .say-shape .say-shape1 {
    position: absolute;
    left: -99px;
    bottom: -140px;
}
@media only screen and (min-width: 1200px) and (max-width: 1440px) {
    .say-something-aera .say-shape .say-shape1 {
    left: -134px;
    bottom: -215px;
}
}.say-something-aera .say-shape .say-shape2 {
    position: absolute;
    right: 0;
    bottom: 0;
}
</style>