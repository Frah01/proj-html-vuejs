<script>

export default {
    props: {
        menuNavBar: Array
    }
}
</script>
<template lang="">
    <div class="container" >
        <div class="row" >
            <div class="col-4">
                <div class="d-flex justify-content-center">
                    <h2>ciao</h2>
                </div>
            </div>
            <div class="col-4">
                <div class="d-flex justify-content-center align-items-center">
                    <ul>
                        <li  v-for="(item, index) in menuNavBar" :key="index" >
                            <a href="">
                                {{item.label}}
                            </a>
                        </li>
                    </ul>
                </div>
                
            </div>
            <div class="col-4">
                <div class="d-flex justify-content-center">
                    <h2>ciao</h2>
                </div>
            </div>
        </div>
        
    </div>
</template>
<style lang="scss" scoped>
@use '../styles/general.scss' as*;
    ul{
        list-style-type: none;
        display: flex;
        padding: 0;
        margin: 0;
        li{
          padding: 5px;
        }
        a{
            text-decoration: none;
            color: black;
        }
    }
</style>