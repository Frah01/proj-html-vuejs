<script>
import AppNavBar from './AppNavbar.vue';
export default {
    components:{
        AppNavBar,
    },
    data(){
        return{
            menuNavBar: [
                {
                    label: 'Home'
                },
                {
                    label: 'Lifestile'
                },
                {
                    label: 'Stories'
                },
                {
                    label: 'Pages'
                },
                {
                    label: 'About us'
                },

            ]
        }
    }
}
</script>
<template lang="">
    <header>
        <AppNavBar :menuNavBar="menuNavBar"/>
    </header>
</template>
<style lang="scss">
    header{
        height: 200px;
        background-color: grey;
    }
</style>