<script>
export default {
    props:{
        contactStarted : Array,
        contactAbout: Array,
        contactFeatures: Array,
        contactLinks: Array,
    }
}
</script>
<template lang="">
    <div class="container p-3" >
    <div class="row" >
        <div class="col-2" >
            <h5>GET STARTED</h5>
            <ul>
                <li v-for="(item,index) in contactStarted" :key="index">
                    {{item.label}}
                </li>
            </ul>
        </div>
        <div class="col-2" >
            <h5>ABOUT</h5>
            <ul>
                <li v-for="(item,index) in contactAbout" :key="index">
                    {{item.label}}
                </li>
            </ul>
        </div>
        <div class="col-2" >
            <h5>FEATURES</h5>
            <ul>
                <li v-for="(item,index) in contactFeatures" :key="index">
                    {{item.label}}
                </li>
            </ul>
        </div>
        <div class="col-2" >
            <h5>QUICK LINKS</h5>
            <ul>
                <li v-for="(item,index) in contactLinks" :key="index">
                    {{item.label}}
                </li>
            </ul>
        </div>
        <div class="col-4" >
            <div class="newslatter d-flex flex-column text-center" >
                <h5>SUBSCRIBE TO NEWSLATTER</h5>
                <input type="text" class="form-control ">
                <button class="btn btn-dark mt-2">SUBSCRIBE</button>
            </div>
        </div>
    </div>
    <hr class="text-white" >
    <div class="row">
        <div class="col">
            <div clas="d-flex justify-content-between" >
                <img src="../" alt="">
            </div>
        </div>
    </div>
   </div>
</template>
<style lang="scss" scoped>
@use '../styles/general.scss' as*;

    ul{
        color: white;
        list-style-type: none;
        padding: 0;
    }

    h5{
        margin-left: 0;
        color: white;
    }

    
</style>