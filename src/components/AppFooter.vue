<script>
import AppSupport from './elements/AppSupport.vue'
export default {
    components:{
        AppSupport,
    },
    data(){
        return{
            contatti: [
                { 
                    title: 'Get started',
                    label: [
                    'Resources',
                    'Tutorials',
                    'Examples',
                    'Docs'
                    ]
                },
                {
                    title: 'About',
                    label: [
                    'Stories',
                    'Community',
                    'Blog',
                    'Brand Assets'
                    ]
                },
                {
                    title: 'Features',
                    label: [
                    'Overview',
                    'Design',
                    'Code',
                    'Collaborate'
                    ]
                },
                {
                    title: 'Quick Links',
                    label: [
                    'Stories',
                    'Community',
                    'Blog',
                    'Brand Assets'
                    ]
                },
                
            ]
        }
    }
}
</script>
<template lang="">
    <footer>
        <AppSupport :contatti="contatti" />
    </footer>
  
</template>
<style lang="scss" scoped>
    footer {
        background-color: rgba(191,29,46,255);
    }
</style>