<template>
   <div>
    <div class="footerUp textFo">
            <img src="/img/logo-svg.svg" alt="logo" class="logo">
           <p>Quam eu proin sit massa condimentum. Volutpat non pulvinar aliquet nunc. <br> Quam eu proin sit massa condimentum.</p>
          <div class="social" v-for="(icon, i) in Social" :class="icon" :key="i"></div>
    </div>
     <div class="footerDown">
        <p> Copyright 2012 - 2022 | Avada Theme by 
            <a href="#">ThemeFusion</a> 
            | All Rights Reserved | Powered by 
            <a href="#">WordPress</a> </p>
     </div>
  </div>
</template>

<script>
    export default {
        name: 'FooterComponent',
        data(){
            return{
                Social: [
                        'fab fa-facebook-f',
                        'fab fa-twitter',
                        'fab fa-youtube',
                        'fab fa-instagram',
                        'fab fa-linkedin-in',
                        ],
                }
         
            }
    }
</script>

<style lang="scss" scoped>
.footerUp {
  width: 100%;
  height: 60vh;
  background: linear-gradient(
      180deg,
      rgba(0, 0, 0, 1) 10%,
      rgba(0, 0, 0, 1) 20%,
      rgba(0, 0, 0, 0.5) 80%
    ),
    url('../assets/image/restaurant.jpg') 100%;
    
    
}
.textFo{
    text-align: center;
    color: white;
   font-size: 1.2rem;
    padding-top: 10%;
}
a {
    text-decoration: none;
    color: white;
}
.social{
      width: 50px;
      height: 50px;
      border-radius: 50%;
      background-color: white;
      color: black;
      display: inline-block;
      padding-top: 15px;
      margin: 5px;
}.social:hover{
    background-color: black;
    color: white;
}

.footerDown{
    background-color: black;
    color: grey;
    padding-bottom: 10px;
    text-align: center;
}
 
</style>