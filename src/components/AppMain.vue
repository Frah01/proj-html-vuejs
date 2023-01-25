<script>
import AppCard from './elements/AppCard.vue'
import AppCardSS from './elements/AppCardSS.vue'
import AppCardTS from './elements/AppCardTS.vue'
import AppCardFS from './elements/AppCardFS.vue'
import AppBanner from './elements/AppBanner.vue'
export default {
    components:{
        AppCard,
        AppCardSS,
        AppCardTS,
        AppBanner,
        AppCardFS,
    },
}
</script>
<template lang="">
    <main>
        <AppCard />
        <AppCardSS />
        <AppCardTS />
        <AppBanner />
        <AppCardFS />
    </main>
</template>

<style lang="">
    
</style>