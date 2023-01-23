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
        <div class="container-fluid" >
            <div class="row">
                <div class="top-bar col-12">
                    <div class="d-flex">
                        <h5>NEWS UPDATES</h5>
                        <h5>5:35</h5>
                        <h5>THE BEST TIME TO HAVE A MEAL</h5>
                    </div>
                    <div>
                        
                    </div>
                </div>
            </div>
        </div>
        <AppNavBar :menuNavBar="menuNavBar"/>
    </header>
</template>
<style lang="scss">
@use '../styles/general.scss' as*;
    header{
        height: 200px;
        background-color: grey;

        .top-bar{
            background-color: rgba(191,29,46,255);
        }

        h5{
            margin-left: 5px;
        }
    }
</style>