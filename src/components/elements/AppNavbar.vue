<script>

export default {
    props: {
        menuNavBar: Array
    }
}
</script>
<template lang="">
    <div class="container p-2" >
        <div class="row" >
            <div class="col-4">
                <div class="d-flex justify-content-center">
                    <i class="fa-solid fa-bars fa-2x"></i>
                </div>
            </div>
            <div class="col-4">
                <div class="d-flex justify-content-center align-items-center">
                    <ul>
                        <li  v-for="(item, index) in menuNavBar" :key="index" :class="item.active ? 'active' : ''">
                            <!-- <div class="dropdown_">
                                <div class="dropbtn">
                                    <a :clas="item.active ? 'active' : ''" >
                                    
                                    </a>
                                </div>
                                    <div class="dropdown-content">
                                        <a href="#">Link 1</a>
                                        <a href="#">Link 2</a>
                                        <a href="#">Link 3</a>
                                    </div>
                                </div> -->
                            <a href="">
                                {{item.label}}
                            </a>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="col-4">
                <div class="d-flex justify-content-center align-items-center">
                    <i class="fa-solid fa-magnifying-glass fa-2x"></i>
                </div>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use '../../styles/general.scss' as*;
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