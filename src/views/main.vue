<script setup>
import MainHeader from "@/components/MainHeader.vue";
import MainFooter from "@/components/MainFooter.vue";
import About from "@/components/About.vue";
import Portfolio from "@/components/Portfolio.vue";
import Contact from "@/components/Contact.vue";
</script>

<template>
    <div class="wrap">
        <MainHeader />
        <div class="inner">
            <About />
            <Portfolio />
            <Contact />
        </div>
        <MainFooter />
    </div>
</template>