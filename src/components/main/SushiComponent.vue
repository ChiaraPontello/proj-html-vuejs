<template>
<div class="navMenu container d-flex align-items-center justify-content-between">
<div class="card text-center" v-for="(link, index) in sushiNav" :key="index">
    <div class="row">
    <img :src="link.imageSushi" class="card-img-top sushi" >
        <div class="card-body">
            <h5 class="card-title">{{ link.title }}</h5>
            <p class="card-text">{{ link.text }}</p>
            <a :href="link.url" class="btn btn-outline-dark">{{ link.urlText }}</a>
        </div>
    </div>
</div>
</div>
</template>

<script>
export default {
    name: 'SushiComponent',
    data() {
        return {
            sushiNav: [
                {   
                    imageSushi: '/img/sushi-1.png',
                    title: 'The best table in town',
                    text: 'Sed aenean egestas ut aliquam turpis mauris, molestie. Vitae tellus tempor sem id tempus neque, tellus turpis turpis. Morbi tortor id gravida aliquet.',
                    url: '#',
                    urlText: 'Explore the menu'
                },
                {   
                    imageSushi: '/img/sushi-2.png',
                    title: 'Perfect For Groups',
                    text: 'Quam eu proin sit massa condimentum. Volutpat non pulvinar aliquet nunc. Orci elementum in aliquet a gravida vivamus aliquam turpis vitae.',
                    url: '#',
                    urlText: 'buy avada today'
                },
                {   
                    imageSushi: '/img/sushi-3.png',
                    title: 'Fresh produce everyday',
                    text: 'Hendrerit amet, volutpat leo non, commodo maecenas scelerisque tincidunt. Morbi vulputate morbi purus quisque sit sagittis orci elementum gravida.',
                    url: '#',
                    urlText: 'Learn more about us'
                },
                
               
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
.navMenu {
    padding: 20px;
    margin: 0 auto;
   
}
.card{
    width: 30%;
    height: 30%;
    border: none;
}

a {
    color: black;
    
    
}


.sushi{
    width: 50%;
    margin-left: 25%;

}

</style>