<script>
import AppCardVF from './AppCardVF.vue';
export default {
    components:{
        AppCardVF,
    },
    data(){
        return{
            thumbCards: [
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
                {
                    img: '../../src/assets/healthy-foods.webp',
                    title: 'The Best Healthy Foods In 2022',
                    text: 'December 26, 2022'
                },
                {
                    img: '../../src/assets/winter.webp',
                    title: 'The Best Winter Outfits',
                    text: 'December 26, 2022'
                },
                {
                    img: '../../src/assets/photographers-mistakes.webp',
                    title: 'Beginner Photographer\'s Mistakes',
                    text: 'December 26, 2022'
                },
                {
                    img: '../../src/assets/visit-france.webp',
                    title: 'Reasons To Visit France',
                    text: 'December 26, 2022'
                },
                {
                    img: '../../src/assets/travel-alone.webp',
                    title: 'Travelling Alone Is Awesome',
                    text: 'December 26, 2022'
                },
                {
                    img: '../../src/assets/success-story.webp',
                    title: 'The best Succes Stories',
                    text: 'December 26, 2022'
                },
            ]
        }
    }
}
</script>
<template lang="">
  <div class="thumb" >
    <div class="container_card d-flex">
            <div class="cards m-2" v-for="(item, index) in thumbCards" :key="index">
                    <AppCardVF :url="item.img" :title="item.title" :text="item.text" />
                </div>
            </div>
  </div>
</template>
<style lang="scss" scoped>

.cards{
    width: calc(100% / 4 - 14px);
}

.thumb {
    background-color: rgba(243,243,243,255);
    overflow-x: scroll;
    padding: 1em;

    h4 {
        text-transform: capitalize;
        margin-top: 10px;
        color: white;
    }

}
</style>