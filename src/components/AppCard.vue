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
                    img: '../assets/best-places-300x200.webp',
                    title: 'Places For a Road Trip',
                    text: 'December 26, 2022'
                },
                {
                    img: '',
                    title: 'Music The Love Of My Life',
                    text: 'December 26, 2022'
                },
                {
                    img: '',
                    title: 'Fashion Trend Now A Days',
                    text: 'December 26, 2022'
                },
                {
                    img: '',
                    title: 'Hygenic Receipe To Prepare Rice',
                    text: 'December 26, 2022'
                },
                {
                    img: '',
                    title: 'The Best Time To Have A Meal',
                    text: 'December 26, 2022'
                },
                {
                    img: '',
                    title: 'The Best Healthy Foods In 2022',
                    text: 'December 26, 2022'
                },
                {
                    img: '',
                    title: 'The Best Winter Outfits',
                    text: 'December 26, 2022'
                },
                {
                    img: '',
                    title: 'Beginner Photographers Mistakes',
                    text: 'December 26, 2022'
                },
                {
                    img: '',
                    title: 'Live Ideas You Might Be Anime',
                    text: 'December 26, 2022'
                },
                {
                    img: '',
                    title: 'Reasons To Visit France',
                    text: 'December 26, 2022'
                },
                {
                    img: '',
                    title: 'Travelling Alone Is Awesome',
                    text: 'December 26, 2022'
                },
                {
                    img: '',
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
    <div class="container_card d-flex flex-wrap justify-content-around">
            <div class="cards m-2" v-for="(item, index) in thumbCards" :key="index">
                    <AppCardVF :url="item.img" :title="item.title" :text="item.text" />
                </div>
            </div>
  </div>
</template>
<style lang="scss" scoped>

.cards{
    width: calc(100% / 4);
    box-shadow: 0 0 6px 3px rgba(0, 0, 0, 0.5);
}
.thumb {
    border: 1px solid black;
    margin: 1em 1em;
    padding: 1em;
    border: 1px solid black;

    h4 {
        text-transform: capitalize;
        margin-top: 10px;
        color: white;
    }

    img {
        box-shadow: 0 0 6px 3px rgba(0, 0, 0, 0.5);
    }
}
</style>