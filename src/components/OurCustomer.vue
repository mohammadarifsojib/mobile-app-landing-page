<template>
    <div>
        <!-- Our Customer Start -->
        <div class="our-customer section-padd-top30">
            <div class="container-fluid">
            <div class="our-customer-wrapper">
                    <!-- Section Tittle -->
                    <div class="row d-flex justify-content-center">
                        <div class="col-xl-8">
                            <div class="section-tittle text-center">
                                <h2 v-html="title"></h2>
                            </div>
                        </div>
                    </div>
                    <div class="row">
                        <div class="col-12">
                            <div class="customar-active dot-style d-flex dot-style flex-column flex-lg-row">
                            
                                <div v-for="customer in ourCustomer" :key="customer.id" class="single-customer mb-100">
                                    <div class="what-img">
                                        <img :src="customer.custPic" alt="{{ customer.custTitle }}">
                                    </div>
                                    <div class="what-cap">
                                        <h4><a :href="customer.custTitleLink">{{ customer.custTitle }}</a></h4>
                                        <p v-html="customer.custComment"></p>
                                    </div>
                                </div>
                            
                            </div>
                        </div>
                    </div>
            </div>
            </div>
        </div>           
        <!-- Our Customer End -->
    </div>
</template>
<script setup>
    import { ref } from 'vue';
    import { ourCustomer } from '../data/ourCustomer.js';
    const title = ref(`What Our Customers<br> Have to Say`)
</script>
<style scoped>
    .our-customer .our-customer-wrapper {
    padding: 0 134px;
}
@media only screen and (min-width: 992px) and (max-width: 1199px) {
    .our-customer .our-customer-wrapper {
    padding: 0 0px;
}
}@media only screen and (min-width: 768px) and (max-width: 991px) {
    .our-customer .our-customer-wrapper {
    padding: 0 0px;
}
}@media (max-width: 767px) {
    .our-customer .our-customer-wrapper {
    padding: 0 0px;
}
}.our-customer .single-customer {
    position: relative;
    margin-left: 15px;
    margin-right: 15px;
    box-shadow: 0px 0px 9px 0px rgba(131, 93, 248, 0.07);
    background: #ffff;
    padding: 55px 34px 55px 44px;
}
@media (max-width: 767px) {
    .our-customer .single-customer {
    padding: 55px 29px 55px 34px;
}
}.our-customer .single-customer .what-img {
    margin-bottom: 20px;
}
.our-customer .single-customer .what-cap h4 a {
    font-size: 20px;
    color: #712fda;
    margin-bottom: 20px;
    text-decoration: none;
}
@media (max-width: 767px) {
    .our-customer .single-customer .what-cap h4 a {
    font-size: 17px;
    text-decoration: none;
}
}.our-customer .single-customer .what-cap h4 a:hover {
    color: #8f1bdc;
}
@media (max-width: 767px) {
    .our-customer .single-customer .what-cap p {
    font-size: 15px;
}
}
</style>