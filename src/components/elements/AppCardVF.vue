<script>
import { defineComponent } from 'vue'
import { Carousel, Pagination, Slide, Navigation } from 'vue3-carousel'
import 'vue3-carousel/dist/carousel.css'
export default {
    components:{
        Carousel,
        Slide,
        Pagination,
        Navigation,
    },
    props: {
        thumbCards: Array,
    }
}
</script>
<template lang="">
    <carousel :autoplay="2500" :itemsToShow="4" :wrapAround="true">
        <slide v-for="(item,index) in thumbCards" :key="index" class="mx-2">
            <div class="d-flex flex-column card border-0" >
                <img class="mb-3 img-fluid" :src="thumbCards[index].img" alt="#">
                <div class="">
                    <h5 class="text-uppercase">{{ thumbCards[index].title }}</h5>
                    <h6>{{  thumbCards[index].text }}</h6>
                    <p class="categoria" >{{thumbCards[index].category}}</p>
                </div>
                
            </div>
        </slide>
        <template #addons>
            <Navigation />
        </template>
    </carousel>
    
</template>
<style lang="scss">

     .carousel .card{
        cursor: pointer;
        h5, h6{
        font-weight: bold;
        position: relative;
        &:hover{
            color: rgba(191,29,46,255);
        }
    }
    }

    .categoria{
        position: absolute;
        top: 5%;
        right: 40%;
        translate: transform(-10%, -50%);
        background-color: white;
        padding: 5px 20px;
        border-radius: 10px;
        font-weight: bold;
        
    }

    img{
        border-radius: 3px 3px 0px 0px,
    }
</style>