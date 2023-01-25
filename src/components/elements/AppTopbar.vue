<script>
export default {
   
}
</script>
<template lang="">
    <div class="container-fluid" >
            <div class="row">
                <div class="top-bar d-flex justify-content-around p-2">
                    <div class="d-flex text-white">
                        <h5>NEWS UPDATES</h5>
                        <h5>5:35</h5>
                        <h5>THE BEST TIME TO HAVE A MEAL</h5>
                    </div>
                    <div class="d-flex align-items-center">
                        <div class="mx-5" >
                            <i class="fa-sharp fa-solid fa-chevron-left text-white"></i>
                            <i class="fa-sharp fa-solid fa-chevron-right text-white"></i>
                        </div>
                        <i class="fa-brands fa-facebook fa-2x "></i>
                        <i class="fa-brands fa-twitter fa-2x "></i>
                        <i class="fa-brands fa-instagram fa-2x"></i>
                        <i class="fa-brands fa-youtube fa-2x"></i>
                    </div>
                </div>
            </div>
        </div>
        <div class="container mt-3" >
            <div class="row" >
                <div class="col-6">
                    <div class="d-flex align-items-center justify-content-start" >
                        <img class="anime-logo" src="../../assets/anime-logo.webp" alt="">
                    </div>
                </div>
                <div class="col-6">
                    <div class="d-flex align-items-center justify-content-center" >
                        <img class="header-logo img-fluid" src="../../assets/header-banner.webp" alt="">
                    </div>
                </div>
            </div>
        </div>
        <hr>
</template>
<style lang="scss">
    @use '../../styles/general.scss' as*;

    .top-bar{
            background-color: rgba(191,29,46,255);
        }

        h5{
            margin-left: 5px;
        }

        .fa-sharp{
            margin-left: 10px; 
            color: white;
            &:hover{
            filter: invert(100%);
        }
        }

        .fa-brands{
        margin-left: 10px; 
        color: white;
        &:hover{
            filter: invert(100%);
        }
        }

        .anime-logo{
            width: 220px;
        }

        .header-logo {
           border-radius: 5px;
        }
</style>