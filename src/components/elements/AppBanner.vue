<script>
import { store } from '../store.js'
export default {
    data(){
        return{
            store,
        }
    }
}
</script>
<template lang="">
    <div class="container-fluid">
        <div class="row p-3">
            <div class="col-12 d-flex justify-content-center">
                <img class="img-fluid" :src="store.advertising.banner" alt="">
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use '../../styles/general.scss' as*;

    .container-fluid{
        background-color: rgba(243,243,243,255);
    }

</style>