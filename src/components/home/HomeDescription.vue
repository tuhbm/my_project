<template>
    <div class="home--descrition">
        <h2>{{ msg }}</h2>
        <h3>구성 View</h3>
        <ol>
            <li>1. 계산기</li>
            <li>2. TODO</li>
            <li>3. 캘린더</li>
            <li>4. 채팅</li>
        </ol>
        <h3>구성 스팩</h3>
        <ol>
            <li>1. Vue.js</li>
            <li>2. Webpack</li>
            <li>3. babel</li>
            <li>4. Vue-router</li>
        </ol>
    </div>
</template>

<script>
    export default {
        name: 'HelloWorld',
        props: ['msg']
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    h2 {
        font-size: 2em;
    }
    h3 {
        font-size: 1.5em;
    }
    h2,
    h3 {
        font-weight: bold;
        margin: 40px 0 0;
    }

    ul {
        list-style-type: none;
        padding: 0;
    }

    li {
        display: inline-block;
        margin: 0 10px;
    }

    a {
        color: #42b983;
    }
</style>
