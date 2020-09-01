<template>
    <header id="header">
        <div class="container">
            <a href="index.html"><img alt="Vue logo" src="../assets/logo.svg"></a>
            <Hamburger/>
            <Navbar/>
        </div>
    </header>
</template>

<script>
import Hamburger from '../assets/Hamburger.vue'
import Navbar from './Navbar.vue'

export default {
    name: 'Header',
    components:{
        Navbar,
        Hamburger
    }
}
</script>

<style scoped>
    #header{
        width:100%;
        background-color: #27A9E1;
    }

    .container{
        width:100%;
        max-width:1200px;
        padding: 15px 10px 8px 10px;
        margin:auto;
        display:flex;
        justify-content:space-between;
        align-items:flex-end;
    }

    a{
        display:flex;
        align-items: flex-end;
    }
</style>