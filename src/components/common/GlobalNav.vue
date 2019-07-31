<template>
    <nav class="nav-global--component">
        <ul class="nav-global--list">
            <li class="nav-global--item" v-for="(item, index) in navList" :key="index+1">
                <i class="nav-global--icon" v-if="item.icon">
                    <img :src="item.icon" :alt="item.title">
                </i>
                <router-link class="nav-global--link" :to="item.link" tag="a">
                    {{item.title}}
                </router-link>
            </li>
        </ul>
    </nav>
</template>

<script>
export default {
    name: "GlobalNav",
    data () {
        return {
            navList: [
                {
                    title: 'Home',
                    link: '/',
                    isNewTab: false,
                    icon: ''
                },
                {
                    title: '계산기',
                    link: '/calculator',
                    isNewTab: false,
                    icon: ''
                },
                {
                    title: 'TODO',
                    link: '',
                    isNewTab: false,
                    icon: ''
                },
                {
                    title: '캘린더',
                    link: '',
                    isNewTab: false,
                    icon: ''
                },
                {
                    title: '채팅',
                    link: '',
                    isNewTab: false,
                    icon: ''
                }
            ]

        };
    }
}
</script>

<style scoped>
.nav-global--component{

}
.nav-global--component .nav-global--list{
    display: flex;
}
.nav-global--component .nav-global--link{
    display: block;
    padding: 2em;
    background: gray;
    color: #fff;
}
.nav-global--component .nav-global--link:hover{
    background: #fff;
    color: #000;
}
.nav-global--component .nav-global--link:before{

}
</style>