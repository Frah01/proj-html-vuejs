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
                    text: 'December 26, 2022',
                    post: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequatur, eos maiores, quasi reprehenderit sunt ratione odio vel ullam earum voluptate nisi, assumenda reiciendis? Laudantium praesentium, blanditiis culpa quisquam explicabo perferendis!'
                },
                {
                    img: '../../src/assets/anime-fashion.webp',
                    title: 'Fashion Trend Now A Days',
                    text: 'December 26, 2022',
                    post: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequatur, eos maiores, quasi reprehenderit sunt ratione odio vel ullam earum voluptate nisi, assumenda reiciendis? Laudantium praesentium, blanditiis culpa quisquam explicabo perferendis!'
                },
                {
                    img: '../../src/assets/rice-ball.webp',
                    title: 'Hygenic Receipe To Prepare Rice',
                    text: 'December 26, 2022',
                    post: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequatur, eos maiores, quasi reprehenderit sunt ratione odio vel ullam earum voluptate nisi, assumenda reiciendis? Laudantium praesentium, blanditiis culpa quisquam explicabo perferendis!'
                },
                {
                    img: '../../src/assets/healthy-foods.webp',
                    title: 'The Best Healthy Foods In 2022',
                    text: 'December 26, 2022',
                    post: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequatur, eos maiores, quasi reprehenderit sunt ratione odio vel ullam earum voluptate nisi, assumenda reiciendis? Laudantium praesentium, blanditiis culpa quisquam explicabo perferendis!'
                },
                {
                    img: '../../src/assets/winter.webp',
                    title: 'The Best Winter Outfits',
                    text: 'December 26, 2022',
                    post: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequatur, eos maiores, quasi reprehenderit sunt ratione odio vel ullam earum voluptate nisi, assumenda reiciendis? Laudantium praesentium, blanditiis culpa quisquam explicabo perferendis!'
                },
                {
                    img: '../../src/assets/photographers-mistakes.webp',
                    title: 'Beginner Photographer\'s Mistakes',
                    text: 'December 26, 2022',
                    post: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequatur, eos maiores, quasi reprehenderit sunt ratione odio vel ullam earum voluptate nisi, assumenda reiciendis? Laudantium praesentium, blanditiis culpa quisquam explicabo perferendis!'
                },
                {
                    img: '../../src/assets/visit-france.webp',
                    title: 'Reasons To Visit France',
                    text: 'December 26, 2022',
                    post: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequatur, eos maiores, quasi reprehenderit sunt ratione odio vel ullam earum voluptate nisi, assumenda reiciendis? Laudantium praesentium, blanditiis culpa quisquam explicabo perferendis!'
                },
                {
                    img: '../../src/assets/travel-alone.webp',
                    title: 'Travelling Alone Is Awesome',
                    text: 'December 26, 2022',
                    post: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequatur, eos maiores, quasi reprehenderit sunt ratione odio vel ullam earum voluptate nisi, assumenda reiciendis? Laudantium praesentium, blanditiis culpa quisquam explicabo perferendis!'
                },
                {
                    img: '../../src/assets/success-story.webp',
                    title: 'The best Succes Stories',
                    text: 'December 26, 2022',
                    post: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequatur, eos maiores, quasi reprehenderit sunt ratione odio vel ullam earum voluptate nisi, assumenda reiciendis? Laudantium praesentium, blanditiis culpa quisquam explicabo perferendis!'
                },
            ]
        }
    }
}
</script>
<template lang="">
  <div class="thumb" >
    <div class="container_card ">
            <div class="cards m-2">
                    <AppCardVF :thumbCards="thumbCards" />
                </div>
            </div>
  </div>
</template>
<style lang="scss" scoped>



.thumb {
    background-color: rgba(243,243,243,255);
    padding: 1em;

    h4 {
        text-transform: capitalize;
        margin-top: 10px;
        color: white;
    }

}
</style>