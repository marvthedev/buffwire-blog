<template>
    <header class="flex">
        <div class="menu">
            <div class="menu__hamburger">
                <div class="menu__bar menu__bar--1"></div>
                <div class="menu__bar menu__bar--2"></div>
                <div class="menu__bar menu__bar--3"></div>
            </div>
        </div>
        <img src="../../assets/images/logo.png" class="flex__logo">
        <div class="flex__search">
            <img src="images/search-regular.svg" class="flex__search--img">
            <input type="search" placeholder="Search" class="flex__search--input">
        </div>
        <nav class="flex__nav">
            <ul>
                <li class="flex__nav--link"><nuxt-link to="/about">About Me</nuxt-link></li>
                <li class="flex__nav--link">My Work</li>
                <li class="flex__nav--link"><nuxt-link to="/blog">Blog</nuxt-link></li>
                <li class="flex__nav--link"><nuxt-link to="/contact">Contact</nuxt-link></li>
            </ul>
        </nav>
    </header>
</template>