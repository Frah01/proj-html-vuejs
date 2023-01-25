<script>
export default {
    props: {
        thumbCards: Array,
    },
    components: {
    
    }
}
</script>
<template lang="">
    <div v-for="(item,index) in thumbCards" class="card container_card m-3 rounded-1 border-0 text-center">
        <img class="mb-3" :src="thumbCards[index].img" alt="#">
        <div class="">
            <h5 class="text-uppercase">{{ thumbCards[index].title }}</h5>
            <h6>{{  thumbCards[index].text }}</h6>
            <p>{{ thumbCards[index].post }}</p>
        </div>
    </div>
</template>
<style lang="">
    
</style>