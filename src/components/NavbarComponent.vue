<script setup>
import { ref } from 'vue';

const isNavOpen = ref(false);

const toggleNav = () => {
    isNavOpen.value = !isNavOpen.value;
};
const closeNav = () => {
    isNavOpen.value = false;
};
</script>

<template>
    <div class="navbar_container">
        <div class="logo">
            <img src="../assets/images/reagan.jpg"  width="35px" height="35px" alt="logo Image">
            <a href="#Hero" @click="closeNav">Radac </a>
        </div>
        <div class="nav_links" :class="{ 'active': isNavOpen }">
            <ul>
                <li><a href="#About" @click="closeNav">About</a></li>
                <li><a href="#Service" @click="closeNav">Services</a></li>
                <li><a href="#Work" @click="closeNav">My work</a></li>
                <li><a href="#Contact" @click="closeNav">Contact</a></li>
            </ul>
        </div>
        <div class="burger" @click="toggleNav" :class="{ 'active': isNavOpen }">
            <span></span>
            <span></span>
            <span></span>
        </div>
    </div>
</template>