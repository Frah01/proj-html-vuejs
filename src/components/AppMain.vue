<script>
import AppCard from './elements/AppCard.vue'
import AppCardSS from './elements/AppCardSS.vue'
import AppCardTS from './elements/AppCardTS.vue'
import AppBanner from './elements/AppBanner.vue'
import AppYoutube from './elements/AppYoutube.vue'
import AppLS from './elements/AppLS.vue'
export default {
    components:{
        AppCard,
        AppCardSS,
        AppCardTS,
        AppBanner,
        AppYoutube,
        AppLS,
    },
}
</script>
<template lang="">
    <main>
        <AppCard />
        <AppCardSS />
        <AppCardTS />
        <AppBanner />
        <AppCard />
        <AppYoutube />
        <AppLS />
    </main>
</template>

<style lang="">
    
</style>