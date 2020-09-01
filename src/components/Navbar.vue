<template>
    <nav id="nav">
        <ul>
            <a href="#">
                <li>Forums</li>
            </a>
            <a href="#">
                <li>News</li>
            </a>
            <a href="#">
                <li>Events</li>
            </a>
            <a href="#">
                <li>About</li>
            </a>
        </ul>
    </nav>
</template>

<script>


export default {
    name: 'Navbar',
}
</script>

<style scoped>
    nav{
        color:white;
        font-size:28px;
    }

    ul{
        list-style: none;
        display:flex;
        flex-direction: row;
    }

    a{
        text-decoration: none;
        color:white;
    }

    li{
        margin-left:25px;
        position:relative;
    }

    li::before{
        content:'';
        width:0%;
        position:absolute;
        bottom:0;
        left:0;
        height:2px;
        background-color:white;
        transition: 0.15s;
    }

    li:hover::before{
        width:100%;
    }

    li:focus::before{
        width:100%;
    }

    li:active::before{
        width:100%;
    }

    @media screen and (min-width: 320px){
        nav{
            display:none;
        }
    }

    @media screen and (min-width: 768px){
        nav{
            display:none;
        }
    }

    @media screen and (min-width: 1200px){
        nav{
            display:block;
        }
    }

</style>