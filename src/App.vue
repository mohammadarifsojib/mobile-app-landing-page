<script setup>
    import Navmenu from './components/Navmenu.vue'
    import HeroSection from './components/HeroSection.vue'
    import BestFeatures from './components/BestFeatures.vue'
    import Services from './components/Services.vue';
    import ApplicApps from './components/ApplicApps.vue'
    import Pricing from './components/Pricing.vue'
    import OurCustomer from './components/OurCustomer.vue'
    import AvailableApps from './components/AvailableApps.vue'
    import SayHello from './components/SayHello.vue'
    import FooterSection from './components/FooterSection.vue'


</script>

<template>
    <div>
        <Navmenu/>
        <main>
            <HeroSection />
            <BestFeatures />
            <Services />
            <ApplicApps />
            <Pricing />
            <OurCustomer />
            <AvailableApps />
            <SayHello />
        </main>
        <FooterSection/>
    </div>
</template>

<style scoped>
  
</style>
