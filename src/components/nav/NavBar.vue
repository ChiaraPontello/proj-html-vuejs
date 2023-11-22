<template>
    <div class="navMenu">
        <div class="text-uppercase container d-flex justify-content-around align-items-center ">
        <img src="src/assets/image/logo-restaurant.png" alt="logo" class="logoAvada">
            <ul class="nav d-flex ">
                <li class="nav-item" v-for="(link, index) in menuNav" :key="index">
                    <div class="d-flex align-items-center">
                        
                        <a class="nav-link" :href="link.url">{{ link.text }}</a>
                        
                    </div>

                </li>
            </ul>
            
        </div>

    </div>
</template>

<script>
export default {
    name: 'menuNav',
    data() {
        return {
            menuNav: [
                {
                    text: 'Home',
                    url: '#',
                },
                {
                    text: 'History',
                    url: '#',
                },
                {
                    text: 'Team',
                    url: '#',
                },
                {
                    text: 'Menu',
                    url: '#',
                },
                {
                    text: 'Takeout',
                    url: '#',
                },
                {
                    text: 'Bulletin',
                    url: '#',
                },
                {
                    text: 'Reservation',
                    url: '#',
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
    z-index: 1000;
}

a {
    color: white;
    float: right;
    margin-top: 0;
}
a:hover{
    color: orange;
}



</style>