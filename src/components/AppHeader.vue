<script>
import AppNavBar from './elements/AppNavbar.vue';
import AppTopbar from './elements/AppTopbar.vue';
export default {
    components:{
        AppNavBar,
        AppTopbar,
    },
    data(){
        return{
            menuNavBar: [
                {
                    icon: `fa-solid fa-house-chimney`,
                    label: 'Home',
                    
                },
                {
                    icon: 'fa-solid fa-suitcase',
                    label: 'Lifestyle',
                    details: [
                    {
                        img: '../../src/assets/best-places.webp',
                        title: 'Places For a Road Trip',
                        text: 'December 26, 2022'
                    },
                    {
                        img: '../../src/assets/anime-fashion.webp',
                        title: 'Fashion Trend Now A Days',
                        text: 'December 26, 2022'
                    },
                    {
                        img: '../../src/assets/rice-ball.webp',
                        title: 'Hygenic Receipe To Prepare Rice',
                        text: 'December 26, 2022'
                    },
                    ]
                },
                {
                    icon: 'fa-solid fa-book-open-reader',
                    label: 'Stories',
                    details: [
                    {
                        img: '../../src/assets/best-places.webp',
                        title: 'Places For a Road Trip',
                        text: 'December 26, 2022'
                    },
                    {
                        img: '../../src/assets/anime-fashion.webp',
                        title: 'Fashion Trend Now A Days',
                        text: 'December 26, 2022'
                    },
                    {
                        img: '../../src/assets/rice-ball.webp',
                        title: 'Hygenic Receipe To Prepare Rice',
                        text: 'December 26, 2022'
                    },
                    ]
                },
                {
                    icon: 'fa-solid fa-book',
                    label: 'Pages'
                },
                {
                    icon: 'fa-solid fa-user',
                    label: 'About us'
                },

            ]
        }
    }
}
</script>
<template lang="">
    <header>
        <AppTopbar />
        <AppNavBar :menuNavBar="menuNavBar"/>
    </header>
</template>
<style lang="scss">
@use '../styles/general.scss' as*;


        .top-bar{
            background-color: rgba(191,29,46,255);
        }

        h5{
            margin-left: 5px;
        }

        .fa-brands{
            margin-left: 10px;
        }
</style>