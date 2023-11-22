<template>
<!--1°MAIN-->
<section class="chef container">
        <!--img roll destra-->
    <div >
<img src="../assets/image/california.jpg" alt="californiaroll" class="california rightBox"><p class="roll">california roll - $22</p>

    </div>

    <!--box sinistra-->
    <div class=" box" >
            <div>
            <p><strong>HAC TELLUS, FELIS RISUS AT mattis mattis.</strong> Eget euismod semper eget tortor, donec amet, blandit. Tristique facilisi faucibus elementum feugiat in nam in feugiat. Ipsum odio etiam duis facilisis amet vulputate. </p>
            <h1 class="text-uppercase">food is our common ground, a universal experience.</h1>
            <p>Tristique tempus condimentum diam donec. Condimentum ullamcorper sit elementum hendrerit mi nulla in consequat, ut. Metus, nullam scelerisque netus viverra dui.</p>
            <img src="../assets/image/signature.jpg" alt="signature" class="signature">
            </div>
    </div>

<!--2°MAIN: SUSHICOMPONENT in cui troviamo le card-->
    <div>
        <SushiComponent />
    </div>
</section>

<!--3°MAIN-->
<section class="experience">
        <!--sezione sinitra-->
        <div >
            <img src="../assets/image/sushiplate.jpg" class="sushiplate">
        </div>
        
        <!--sezione destra-->
        <div class="rightSection " >
            <div class="fineDinning">
            <span class="text-uppercase">the best table in town </span>
            <h1 class="text-uppercase">fine dining experience</h1>
            <p>Pellentesque vitae viverra risus, sagittis. Venenatis ridiculus scelerisque nisi in urna nulla. Sit tempor a et nisl, ac felis.</p>
            
            <button type="button" class="btn btn-outline-light buy">BUY AVADA TODAY</button>
            </div>
        </div>
        
    </section>

    <!--4°MAIN: CriticsComponenet-->
    <CardCritic />
    
</template>

<script>
import SushiComponent from './main/SushiComponent.vue';
import CardCritic from './main/CardCritic.vue';
    export default {
        name: 'MainComponent',
        components: {
            SushiComponent,
            CardCritic,
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
.roll{
    position: absolute;
    padding-left: 60%;
    padding-top:42%;
    color: white;
    font-size: 2rem;
}

.rightBox:hover {
      transition: transform 0.5s;
      transform: scale(1.04);
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

.experience{
    background-color: black;
    margin-bottom: 100px;
}
.sushiplate{
    width: 60%;
    height: 80vh;
    float: left;
}
.rightSection{
    width: 80%;
    height: 80vh;
}
.fineDinning{
    padding-top: 10%;
    color: white;
    
}

</style>