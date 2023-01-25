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
                <a class="btn" data-bs-toggle="offcanvas" href="#offcanvasExample" role="button" aria-controls="offcanvasExample">
                    <div class="d-flex justify-content-center">
                        <i class="fa-solid fa-bars fa-2x"></i>
                    </div>
                </a>
                    <div class="offcanvas w-25 offcanvas-start" tabindex="-1" id="offcanvasExample" aria-labelledby="offcanvasExampleLabel">
                    <div class="offcanvas-header">
                        <h5 class="offcanvas-title" id="offcanvasExampleLabel"></h5>
                        <button type="button" class="btn-close text-reset" data-bs-dismiss="offcanvas" aria-label="Close"></button>
                    </div>
                    <div class="offcanvas-body">
                        <div class="container">
                            <div class="row ">
                                <div class="col">
                                    <div class="d-flex justify-content-center">
                                        <img class="img-fluid" src="../../assets/anime-logo.webp" alt="">
                                    </div>
                                    <div>
                                        <p class="text-center">Lorem ipsum dolor sit amet consectetur adipisicing elit. Nemo amet, eaque doloremque iste consequatur delectus esse fuga. Omnis consequuntur minus cum voluptatem sed facilis quo sint harum tempora doloremque. Saepe?</p>
                                    </div>
                                    <div class="d-flex justify-content-center">
                                        <img  class="img-fluid img-w mx-1" src="../../assets/visit-france.webp" alt="">
                                        <img  class="img-fluid img-w mx-1" src="../../assets/visit-france.webp" alt="">
                                        <img  class="img-fluid img-w mx-1" src="../../assets/visit-france.webp" alt="">
                                    </div>
                                    
                                </div>
                            </div>
                        </div>
                        
                    </div>
                    </div>
               
            </div>
            <div class="col-4">
                <div class="d-flex justify-content-center align-items-center">
                    <ul>
                        <li v-for="(item, index) in menuNavBar" :key="index" :class="item.active ? 'active' : ''">
                            <a href="">
                                <i :class="item.icon" ></i>
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

    .offcanvas{
        .img-w{
            width: 120px;
            
        }
    }
</style>