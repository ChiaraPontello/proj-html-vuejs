<template>
    <div id="App">
        <HeaderComponent />
        <MainComponent />
        <FooterComponent />
    </div>    
       
    
    
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
import FooterComponent from './components/FooterComponent.vue';
    export default {
        name: 'App',
        components: {
            HeaderComponent,
            MainComponent,
            FooterComponent,
        }
        
    }
</script>

<style lang="scss" scoped>

  @import url('https://fonts.googleapis.com/css2?family=Kanit:wght@700&family=Lato:wght@100;300;400&family=Montserrat:wght@400;600&family=Noto+Sans:wght@300;600&family=PT+Sans:wght@400;700&family=Roboto:wght@300;500;900&display=swap');
  @import url("https://use.fontawesome.com/releases/v5.7.1/css/all.css");
</style>