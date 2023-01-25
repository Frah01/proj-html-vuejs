<script>
import { store } from '../store.js'
export default {
    data(){
        return{
            store,
        }
    }
}
</script>
<template lang="">
     <div class="container-fluid py-5">
        <div class="row">
            <div class="col-12 d-flex justify-content-around align-items-center">
                <div id="background-img-1" class="card backg-img border-0 rounded mt-2 d-flex justify-content-center align-items-center">
                    <div class="content" >
                       <h3>Fashoin</h3>
                    </div>
                </div>
                <div id="background-img-2" class="card backg-img border-0 rounded mt-1 d-flex justify-content-center align-items-center" >
                    <div class="content">
                       <h3>Food</h3>
                    </div>
                </div>
            
                <div id="background-img-3" class="card border-0 backg-img rounded d-flex justify-content-center align-items-center" >
                    <div class="content">
                        <h3>Travel</h3>
                    </div>
                </div>
                <div id="background-img-4" class="card backg-img border-0 rounded mt-2 d-flex justify-content-center align-items-center">
                    <div class="content" >
                       <h3>Lifestyle</h3>
                    </div>
                </div>
                <div id="background-img-5" class="card backg-img border-0 rounded mt-1 d-flex justify-content-center align-items-center ">
                    <div class="content">
                       <h3>Food</h3>
                    </div>
                </div>
                <div id="background-img-6" class="card backg-img border-0 rounded mt-1 d-flex justify-content-center align-items-center ">
                    <div class="content">
                       <h3>Culture</h3>
                    </div>
                </div>
            </div>
        </div>
    </div>
    
</template>
<style lang="scss" scoped>
   
   .backg-img{
        width: 250px;
        height: 250px;
        background-size: cover;
        background-repeat: no-repeat;
        filter: brightness(60%);
        text-align: center;
        color: white;
        transition: 0.5s linear;

        &:hover{
            filter: brightness(100%);
        }
    }

    .content{
        width: 177px;
        h3{
            text-transform: uppercase;
        }
    }


    #background-img-1{
        background-image: url('../../assets/anime-fashion.webp');
        
    }
    #background-img-2{
        background-image: url('../../assets/travel-alone.webp');

        
    }
    #background-img-3{
        background-image: url('../../assets/best-places.webp');

        
    }
    #background-img-4{
        background-image: url('../../assets/visit-france.webp');

        
    }
    #background-img-5{
        background-image: url('../../assets/healthy-foods.webp');

        
    }

    #background-img-6{
        background-image: url('../../assets/success-story.webp');

        
    }
</style>