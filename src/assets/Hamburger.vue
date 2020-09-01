<template>
    <div class="hamburger" id="hamburger">
        <div class="hamburger-line"></div>
        <div class="hamburger-line"></div>
        <div class="hamburger-line"></div>
    </div>
</template>

<script>
export default {
    name:'Hamburger'    
}
</script>

<style scoped>
    .hamburger{
        height:40px;
        max-width:46px;
        width:100%;
        flex-direction: column;
        justify-content: space-between;
        padding-bottom:5px;
    }

    .hamburger-line{
        height:6px;
        width:100%;
        background-color:white;
    }

    @media screen and (min-width: 320px){
        .hamburger{
            display:flex;
        }
    }

    @media screen and (min-width: 768px){
        .hamburger{
            display:flex;
        }
    }

    @media screen and (min-width: 1200px){
        .hamburger{
            display:none;
        }
    }
</style>