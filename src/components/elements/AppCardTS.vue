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
   <div class="container py-5" >
    <div class="row py-4">
        <div class="col d-flex justify-content-between">
            <div>
                <h3 class="text-uppercase">Lifestyle & stories</h3>
            </div>
            <div>
                <button class="btn btn-dark mx-1">ALL</button>
                <button class="btn btn-dark mx-1">LIFESTILE</button>
                <button class="btn btn-dark mx-1">STORIES</button>
            </div>
            
        </div>
    </div>
    <div class="row" >
        <div class="col-8">
                 <div id="background-img-1" class="backg-img  rounded d-flex align-items-end mt-1" >
                    <div class="content">
                        <h6>{{store.info[8].demo}} {{store.info[8].text}}</h6>
                        <h5>{{store.info[8].title}}</h5>
                        <p class="categoria" >{{store.info[8].category}}</p>

                    </div>
                 </div>
            
           
        </div>
        <div class="col-4">
            <div class="box">
                <div id="background-img-2" class="backg-img-sm rounded d-flex align-items-end mt-1" ></div>
            <div class="content">
                    <h6>{{store.info[7].demo}} {{store.info[7].text}}</h6>
                    <h5>{{store.info[7].title}}</h5>
                    <p class="categoria" >{{store.info[7].category}}</p>
                </div>
            </div>
            
            <hr>
            <div class="box">
                <div id="background-img-3" class=" backg-img-sm rounded d-flex align-items-end mt-1" ></div>
                 <div class="content">
                    <h6>{{store.info[0].demo}} {{store.info[0].text}}</h6>
                    <h5>{{store.info[0].title}}</h5>
                    <p class="categoria" >{{store.info[0].category}}</p>
                </div>
            </div>
            <hr>
            <div class="box">
                 <div id="background-img-4" class=" backg-img-sm rounded d-flex align-items-end mt-1" ></div>
                 <div class="content">
                    <h6>{{store.info[6].demo}} {{store.info[6].text}}</h6>
                    <h5>{{store.info[6].title}}</h5>
                    <p class="categoria" >{{store.info[6].category}}</p>
                </div>
            </div>
        </div>
    </div>
   </div>
</template>
<style lang="scss" scoped>
@use '../../styles/general.scss' as*;
@use '../../styles/partials/mixins.scss' as*;
.backg-img{
        aspect-ratio: 400 / 205;
        background-size: contain;
        filter: brightness(60%);

        &:hover{
            filter: brightness(100%);
        }
        .content{
            color: white;
            padding: 10px;
            h6{
                margin-left: 5px;
            }
        }
    }
    .categoria{
        color: black;
        @include categoria;
    }
    

    .content{
        width: 177px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        h6{
            margin-left: 5px;
            font-size: 12px;
            
        }
        h5{
            font-size: 16px;
        }
    }
.backg-img-sm{
        position: relative;
        width: 177px;
        aspect-ratio: 177 / 119;
        background-size: contain;
        filter: brightness(60%);
        &:hover{
            filter: brightness(100%);
        }
        .content{
            padding: 10px;
            text-align: center;
        }
}


.box{
    display: flex;
}


    #background-img-1{
        background-image: url('../../assets/success-story.webp');
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
</style>