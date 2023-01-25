<script>
export default {
    props:{
        contatti: Array,
    }
}
</script>
<template lang="">
    <div class="container p-3" >
    <div class="row" >
        <div class="container">
            <div class="row">
                <div class="col-8">
                    <ul class="d-flex">
                        <li class="mx-3" v-for="(item,index) in contatti " :key="index">{{item.title}}
                            <ul>
                                <li v-for="(item,index) in item.label" :key="index" >{{item}}</li>
                            </ul>
                        </li>
                    </ul>
                </div>
                <div class="col-4" >
                    <div class="newslatter d-flex flex-column text-center" >
                        <h5>SUBSCRIBE TO NEWSLATTER</h5>
                        <input placeholder="Email" type="email" class="form-control ">
                        <button class="btn btn-dark mt-2">SUBSCRIBE</button>
                    </div>
        </div>
            </div>
        </div>
        
        
    </div>
    <hr class="text-white" >
    <div class="row">
        <div class="col d-flex justify-content-between align-items-center">
            <div >
                <img class="logo-footer" src="../../assets/anime-whitelogo.png" alt="">
            </div>
            <div>
                <a href="">© Anime Tech, Theme by Fra</a>
            </div>
        </div>
    </div>
   </div>
</template>
<style lang="scss" scoped>
@use '../../styles/general.scss' as*;

    ul{
        color: white;
        list-style-type: none;
        padding: 0;
        line-height: 35px;
    }

    h5{
        margin-left: 0;
        color: white;
    }

    .logo-footer{
        width: 230px;
    }

    a{
        text-decoration: none;
        color: white;
    }

    
</style>