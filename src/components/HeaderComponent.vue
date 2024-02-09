<template>
    <!--sezione destra-->
    <header class="intro">
        <NavBar />
        <div >
            <img src="../assets/image/restaurant.jpg" class="restaurant">
        </div>
        
        <!--sezione sinistra-->
        <div class="leftSection " >
            <div class="fusion">
            <span class="text-uppercase">the best table in town </span>
            <h1 class="text-uppercase">fine dining experience</h1>
            <p>Pellentesque vitae viverra risus, sagittis. Venenatis ridiculus scelerisque.</p>
            
            <button class="btn btn-outline-light buy">BUY AVADA TODAY</button>
            </div>
        </div>
    </header>
</template>

<script>
import NavBar from './nav/NavBar.vue'
    export default {
        name: 'HeaderComponent',
        components: {
            NavBar,
        }
    }
</script>

<style lang="scss" scoped>
.intro {
    background-color: black;
}
hr{
    margin-right: 40px;
    width: 60px;
    color: white;
}
.restaurant{
    width: 50%;
    height: 100vh;
    float: right;
   
}
p{
    color: white;
    padding: 10px;
    font-size: 1.3rem;
}
h1{
    color: white;
    font-size: 5rem;
}
span{
    color: white;
    font-size: 1.5rem;
}
.leftSection{
width: 100%;
height: 100vh;
}
.fusion{
    padding-top: 10%;
    padding-left: 10%;
    
}

</style>

