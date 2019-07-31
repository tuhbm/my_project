<template>
    <header class="gnb--component">
        <h1 class="gnb--logo">
            <router-link class="gnb--link" to="/" tag="a">
                <img src="../../assets/logo-ktk.png" alt="ktk">
            </router-link>
        </h1>
        <global-nav></global-nav>
    </header>
</template>

<script>

import GlobalNav from './GlobalNav';

export default {
    name: "Gnb",
    components: {
        GlobalNav
    }
}
</script>

<style>
.gnb--component {
    display: flex;
    width: 100%;
    background: gray;
    border-bottom:1px solid #000;
}
.gnb--component + div,
.gnb--component + section {
    margin-top: 50px;
}
.gnb--logo{
    display:inline-block;
    width: 5em;
    height: 5em;
    margin: 0.2em 3em 0.2em 0.2em;
}
.gnb--link{
    display: block;
}
.gnb--logo img{
    width: 100%;
    height: auto;
}
</style>