<script setup>
import { headerNav } from "@/constants/list";
import { ref, onMounted } from "vue";

var headerHeight = document.querySelector('.header');

const isMenuOpen = ref(false);
const isHeaderFixed = ref(false);

const toggleMenu = () => {
  if (window.innerWidth <= 1080) {
    isMenuOpen.value = !isMenuOpen.value;
  }
};

onMounted(() => {
  window.addEventListener("scroll", handleScroll);
});

const handleScroll = () => {
  isHeaderFixed.value = window.scrollY > headerHeight;
};

// 링크 스크롤 이벤트
window.addEventListener("DOMContentLoaded", function() {
    var speed = 500;  // 스크롤 스피드 수치로 사용할 변수

    // 로직
    function scrolling(obj) {
        if (!obj) {
            window.scrollTo({ top: 0, behavior: "smooth" });
        } else {
            var targetElement = document.querySelector(obj);
            if (targetElement) {
                var posTop = targetElement.getBoundingClientRect().top + window.scrollY - headerHeight;
                window.scrollTo({ top: posTop, behavior: "smooth" });
            }
        }
    }

    var navLinks = document.querySelectorAll(".navList__link");
    navLinks.forEach(function(link) {
        link.addEventListener("click", function(event) {
            event.preventDefault();
            var direction = link.getAttribute("href");
            scrolling(direction);
        });
    });

    var logo = document.querySelector(".logo"); // 로고 요소 선택
    if (logo) {
        logo.addEventListener("click", function(event) {
            event.preventDefault();
            scrolling(null);
        });
    }
});

</script>

<template>
    <header class="header" :class="{ act: isHeaderFixed }">
        <nav class="nav">
            <div class="nav__inner">
                <a href="#none" class="logo"><span class="blind">K</span>IM BORA</a>
                <button class="menuBtn mobile" :class="{ on: isMenuOpen }" @click="toggleMenu">
                    <span class="blind">메뉴버튼</span>
                    <i class="bar"></i>
                </button>
                <ul class="navList" :class="{ on: isMenuOpen }" @click="toggleMenu">
                    <li class="navList__item" v-for="(nav, key) in headerNav" :key="key">
                        <a class="navList__link" :href="nav.url">{{ nav.title }}</a>
                    </li> 
                </ul>
            </div>
        </nav>
    </header>

</template>