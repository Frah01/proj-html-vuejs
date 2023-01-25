<script>
import {store} from '../store.js'
export default {
    data(){
        return{
            store,
        }
    }
}
</script>
<template lang="">
    <div class="container py-5">
        <div class="row">
            <div class="col-3">
                <div id="background-img-1" class="card backg-img border-0 rounded mt-2 d-flex justify-content-end">
                    <div class="content" >
                        {{store.info[1].demo}}
                        {{store.info[1].text}}
                        <h5>{{store.info[1].title}}</h5>
                    </div>
                </div>
                <div id="background-img-2" class="card backg-img border-0 rounded mt-1 d-flex justify-content-end" >
                    <div class="content">
                        {{store.info[7].demo}}
                        {{store.info[7].text}}
                        <h5>{{store.info[7].title}}</h5>
                    </div>
                </div>
            </div>
            <div class="col-6">
                <div id="background-img-3" class="card border-0 backg-img rounded p-2 d-flex justify-content-end" >
                    <div class="content">
                        {{store.info[0].demo}}
                        {{store.info[0].text}}
                        <h5>{{store.info[0].title}}</h5>
                    </div>
                </div>
            </div>
            <div class="col-3">
                <div id="background-img-4" class="card backg-img border-0 rounded mt-2 d-flex justify-content-end">
                    <div class="content" >
                        {{store.info[6].demo}}
                        {{store.info[6].text}}
                        <h5>{{store.info[6].title}}</h5>
                    </div>
                </div>
                <div id="background-img-5" class="card backg-img border-0 rounded mt-1 d-flex justify-content-end ">
                    <div class="content">
                        {{store.info[3].demo}}
                        {{store.info[3].text}}
                        <h5>{{store.info[3].title}}</h5>
                    </div>
                </div>
                
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
    @use '../../styles/general.scss' as*;

    .backg-img{
        aspect-ratio: 500 / 333;
        background-size: contain;
        filter: brightness(60%);
        text-align: center;
        color: white;
        transition: 0.5s linear;

        &:hover{
            filter: brightness(100%);
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


    img{
        border-radius: 3px;
        opacity: 0.8;
    }
</style>