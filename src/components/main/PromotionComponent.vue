<template>
<div class="container">
      <!-- title-->
    <div class="title">
      <p><i> Latest News & Promotions </i></p>
      <hr>
    </div>

    <!-- promotionBox-->
    <div class="d-flex justify-content-between text-center">

    <!--1°box-->
      <div class="card">
        <img src="/img/drink.jpg" alt="drink">
        <div class="shadowBox">
        <!--scompare all'hover-->
         <div class="hiddenBox">
          <h2 class="text-uppercase py-4">The best coffe in town</h2>
          <p>By admin | January 7th, 2020 | Categories: News</p>
        </div>
        <!--compare hover-->
        <div class="textCard">
          <i class="fas fa-link"></i>
          <h4 class="text-uppercase">The best coffe in town</h4>
          <p>News</p>
        </div>
        </div>
      </div>

      <!--2°box-->
      <div class="card">
        <img src="/img/girl.jpg" alt="girl">
        <div class="shadowBox">
        <!--scompare all'hover-->
         <div class="hiddenBox">
          <h2 class="text-uppercase py-3">Discover our new menu</h2>
          <p>By admin | January 7th, 2020 | Categories: News</p>
        </div>
        <!--compare all'hover-->
        <div class="textCard">
          <i class="fas fa-link"></i>
          <h4 class="text-uppercase">Discover our menu</h4>
          <p>News</p>
        </div>
        </div>
      </div>

      <!--3°box-->
      <div class="card">
        <img src="/img/pos.jpg" alt="pos">
        <div class="shadowBox">
        <!--scompare all'hover-->
        <div class="hiddenBox">
                <h2 class="text-uppercase py-3">We now accept square!</h2>
                <p>By admin | January 7th, 2020 | Categories: News</p>
            </div>
        <!--compare all'hover-->
        <div class="textCard">
          <i class="fas fa-link"></i>
          <h4 class="text-uppercase">We now accept square!</h4>
          <p>News</p>
        </div>
        
            
        </div>
      </div>

    </div>

</div>

</template>

<script>
    export default {
        name:'PromotionComponent',
    }
</script>

<style lang="scss" scoped>

.title {
  text-align: center;
  padding-bottom: 5%;
  padding-top: 5%;
  font-size: 3rem;
}
hr{
    margin-right: 40px;
    width: 20%;
    color: black;
    margin-left: 40%;
}


//blocco card 
  .card {
    position: relative;
    width: 30%;
    height: 90vh;
    
    img {
      position: absolute;
      width: 100%;
      height: 90vh;
      right: 1px;
      object-fit: cover;
    }
    
    .shadowBox {
      position: absolute;
      width: 100%;
      height: 90vh;
    } &:hover .shadowBox {
        background: linear-gradient(
          180deg,
          rgba(0, 0, 0, 0.8) 0%,
          rgba(255, 255, 255, 0) 95%
        );
      }
    
    .hiddenBox {
      color: black;
      position: absolute;
      bottom: 0;
      background-color: white;
    }&:hover .hiddenBox {
        height: 0px;
        overflow: hidden;
      }
    .textCard {
      position: absolute;
      color: white;
      margin-top: 50%;
      margin-left: 15%;
      text-align: center;
      display: none;
    } &:hover .textCard{
        display: block;
        color: white;
    }
    }
  

</style>