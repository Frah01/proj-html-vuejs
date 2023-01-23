<script>
export default {
    props: {
        url: String,
        title: String,
        text: String
    }
}
</script>
<template lang="">
    <div class="card rounded-1 border-1  h-100 text-center">
        <img class="mb-3" :src="url" alt="#">
        <div class="h-100 d-flex flex-column justify-content-between">
            <h5 class="text-uppercase">{{ title }}</h5>
            <h6>{{ text }}</h6>
        </div>
    </div>
</template>
<style lang="">
    
</style>