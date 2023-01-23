<script>
import AppNavBar from './AppNavbar.vue';
import AppTopbar from './AppTopbar.vue';
export default {
    components:{
        AppNavBar,
        AppTopbar,
    },
    data(){
        return{
            menuNavBar: [
                {
                    icon: '<i class="fa-solid fa-house-chimney"></i>',
                    label: 'Home'
                },
                {
                    icon: '<i class="fa-solid fa-house-chimney"></i>',
                    label: 'Lifestyle'
                },
                {
                    icon: '<i class="fa-solid fa-house-chimney"></i>',
                    label: 'Stories'
                },
                {
                    icon: '<i class="fa-solid fa-house-chimney"></i>',
                    label: 'Pages'
                },
                {
                    icon: '<i class="fa-solid fa-house-chimney"></i>',
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