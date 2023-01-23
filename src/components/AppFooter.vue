<script>
import AppSupport from './AppSupport.vue'
export default {
    components:{
        AppSupport,
    },
    data(){
        return{
            contactStarted: [
                {
                    label: 'Resuorces'
                },
                {
                    label: 'Tutorials'
                },
                {
                    label: 'Examples'
                },
                {
                    label: 'Docs'
                },
            ],
            contactAbout: [
                {
                    label: 'Stories'
                },
                {
                    label: 'Community'
                },
                {
                    label: 'Blog'
                },
                {
                    label: 'Brand Assets'
                },
            ],
            contactFeatures: [
                {
                    label: 'Overview'
                },
                {
                    label: 'Design'
                },
                {
                    label: 'Code'
                },
                {
                    label: 'Collaborate'
                },
            ],
            contactLinks : [
                {
                    label: 'Stories'
                },
                {
                    label: 'Community'
                },
                {
                    label: 'Blog'
                },
                {
                    label: 'Brand Assets'
                },
            ],
            
        }
    }
}
</script>
<template lang="">
    <footer>
        <AppSupport :contactStarted="contactStarted" :contactAbout="contactAbout" :contactFeatures="contactFeatures" :contactLinks="contactLinks" />
    </footer>
  
</template>
<style lang="scss" scoped>
    footer {
        height: 300px;
        background-color: rgba(191,29,46,255);
    }
</style>