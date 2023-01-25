<script>

export default {
    data(){
        return{
            methods:{
                myclick(){

                }
            }
        }
    },
    props: {
        menuNavBar: Array
    }
}
</script>
<template lang="">
    <div class="container p-2" >
        <div class="row my-2" >
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
                                        <img  class="img-fluid img-w mx-1" src="../../assets/best-places.webp" alt="">
                                        <img  class="img-fluid img-w mx-1" src="../../assets/visit-france.webp" alt="">
                                        <img  class="img-fluid img-w mx-1" src="../../assets/photographers-mistakes.webp" alt="">
                                    </div>
                                    <div class="d-flex flex-column align-items-center mt-3 h4">
                                        <p>Sun - Sat : 9:00 AM - 18:00 PM</p>
                                        <p>contact@domain.com</p>
                                        <p>(+82) 8123 456 789</p>
                                    </div>
                                    <div class="d-flex justify-content-center">
                                        <i class="fa-brands fa-facebook fa-2x text-danger"></i>
                                        <i class="fa-brands fa-twitter fa-2x text-danger"></i>
                                        <i class="fa-brands fa-instagram fa-2x text-danger"></i>
                                        <i class="fa-brands fa-youtube fa-2x text-danger"></i>
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
                    <div class="search-box">
                        <button class="btnn-search"><i class="fas fa-search"></i></button>
                        <input type="text" class="input-search" placeholder="Cerca...">
                    </div>
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
          font-weight: bold;
        }
        a{
            text-decoration: none;
            color: black;

            &:hover{
                color: rgba(191,29,46,255);
            }
        }
    }

    .fa-bars, .fa-magnifying-glass{
        &:hover{
            color: rgba(191,29,46,255);
        }
    }

    .offcanvas{
        .img-w{
            width: 120px;
            
        }
    }


 .search-box{
  width: fit-content;
  height: fit-content;
  position: relative;
}
.input-search{
  height: 50px;
  width: 50px;
  border-style: none;
  padding: 10px;
  font-size: 18px;
  letter-spacing: 2px;
  outline: none;
  border-radius: 25px;
  transition: all .5s ease-in-out;
  background-color: black;
  padding-right: 40px;
  color:#fff;
}
.input-search::placeholder{
  color:rgba(255,255,255,.5);
  font-size: 18px;
  letter-spacing: 2px;
  font-weight: 100;
}
.btnn-search{
  width: 50px;
  height: 50px;
  border-style: none;
  font-size: 20px;
  font-weight: bold;
  outline: none;
  cursor: pointer;
  border-radius: 50%;
  position: absolute;
  right: 0px;
  color:#ffffff ;
  background-color:transparent;
  pointer-events: painted;  
}
.btnn-search:focus ~ .input-search{
  width: 300px;
  border-radius: 0px;

  border-bottom:1px solid rgba(255,255,255,.5);
  transition: all 500ms cubic-bezier(0, 0.110, 0.35, 2);
}
.input-search:focus{
  width: 300px;
  border-radius: 0px;
  
  border-bottom:1px solid rgba(255,255,255,.5);
  transition: all 500ms cubic-bezier(0, 0.110, 0.35, 2);
}
</style>