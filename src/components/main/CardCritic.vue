<template>
  <div>
      <div class="container">
        <!-- titolo-->
        <div class="title text-center">
          <p><i> What critics are saying about us </i></p>
        </div>
  
        <!-- MEGGY SINISTRA-->

        <div class="meggy">
          
          <img src="/img/girl.jpg" alt="" class="girl">
          
          <div class="rightBox ">
           <!--DESTRA-->
            <div class="textBox">
              <h4>MEGGY STEWART</h4>
              <h1>NEW YORK TIMES</h1>
              <hr>
              <p>Non arcu mauris tortor ultrices mollis tellus euismod fermentum. Habitant amet tincidunt id sapien accumsan sed at.</p>
              <p>Mmalesuada ullamcorper amet. Pretium pretium dignissim nisi</p>
              <button class="btn btn-outline-light buy">READ FULL ARTICLE</button>
            </div>
          </div>
        </div>
      
        <!--box guardian -->
      <div class="d-flex justify-content-between ">
        <div class="boxLeft ">
          <div class="textBox text-light ">
            <h4>MARY MAXEY</h4>
            <h1>THE GUARDIAN</h1>
            <hr>
            <p>Non arcu mauris tortor ultrices mollis tellus euismod fermentum. Habitant amet tincidunt id sapien accumsan sed.</p>
            <button class="btn btn-outline-light buy">READ FULL ARTICLE</button>
          </div>
        </div>
      
        <!-- box globe -->
      <div class="boxRight ">
        <div class="textBox text-light">
            <h4>PATRICK MONROE</h4>
            <h1>GLOBE AND MAIL</h1>
            <hr>
            <p>Vivamus magna justo, lacinia eget consectetur sed, convallis at tellus. Nulla porttitor accumsan tincidunt.</p>
            <button class="btn btn-outline-light buy">READ FULL ARTICLE</button>
        </div>
      </div>
    </div>
    </div>

  <!--img kungpao-->
    <div class="imgkung">
      <img src="/img/kungpao.jpg" alt="" class="kung">
      <h3 class="textKung">KUNG PAO CHICKEN - $32</h3> 
    </div>
  </div>
  </template>

<script>
  export default {
    name: 'CardCritic',
  }
</script>

<style lang="scss" scoped>
.girl{
  width: 50%;
}
.title{
  padding-bottom: 20px;
  font-size: 3rem;
}
hr{
    margin-right: 40px;
    width: 60px;
}
.meggy {
  display: flex;
}
.textBox{
 padding-left: 100px;
 margin-top: 30%;
 h1{
  font-size: 3rem;
  padding-bottom: 40px;
 }
 p{
  font-size: 1.5rem;
 }
}
.rightBox {
    width: 50%;
    background-color: black;
    color: white;
    &:hover {
      transition: transform 0.5s;
      transform: scale(1.04);
    }
  }
  .boxLeft {
  background-image: url('/img/girl2.jpg');
  background-size: cover;
  width: 45%;
  height: 90vh;
  padding: 40px;
  margin-top: 30px;
}
.boxRight {
  background-image: url('/img/boys.jpg');
  background-size: cover;
  width: 45%;
  height: 90vh;
  padding: 40px;
  margin-top: 30px;
  float: right;
  
}

.imgkung {
  position: relative;
  
  .kung{
    width: 100%;
    padding-top: 50px;
   
  }
  .textKung{
    position: absolute;
    bottom: 2px;
    left: 40%;
    color: white;
}
}


</style>