<template>
    <main class="chef container">
    <div >
<img src="../assets/image/california.jpg" alt="californiaroll" class="california">
    </div>

    <!--sezione sinistra-->
    <div class=" box" >
            <div>
            <p><strong>HAC TELLUS, FELIS RISUS AT mattis mattis.</strong> Eget euismod semper eget tortor, donec amet, blandit. Tristique facilisi faucibus elementum feugiat in nam in feugiat. Ipsum odio etiam duis facilisis amet vulputate. </p>
            <h1 class="text-uppercase">food is our common ground, a universal experience.</h1>
            <p>Tristique tempus condimentum diam donec. Condimentum ullamcorper sit elementum hendrerit mi nulla in consequat, ut. Metus, nullam scelerisque netus viverra dui.</p>
            <img src="../assets/image/signature.jpg" alt="signature" class="signature">
            </div>
    </div>

    <div>
        <SushiComponent />
    </div>
    </main>
</template>

<script>
import SushiComponent from './sushi/SushiComponent.vue';
    export default {
        name: 'MainComponent',
        components: {
            SushiComponent,
        }
    }
</script>

<style lang="scss" scoped>
.chef {
    padding-top:50px;
    padding-bottom: 20px;
    
}
.california{
    width: 40%;
    height: 40%;
    float: right;
}

h1{
    font-size: 3.2rem;
    padding-bottom: 20px;
}
p {
    font-size: 1.2rem;
    padding-bottom: 20px;
    
}
.box{
    height: 40%;
    width: 40%;
    padding-top: 10%;
}
.signature{
    width: 50%;
}
</style>