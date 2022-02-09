<template>

    
        <div class="col-2">
            <img :src="thumb" class="image" :alt="series">
            <div class="card-text my-2">
                {{series}}
             </div>
        </div>
  
    

</template>

<script>
export default {
 name:'Card',
 props:['thumb','series'],
}
</script>

<style lang="scss" scoped>

@import "./../assets/scss/index.scss";


.card-text
{
    color: white;
    text-transform: uppercase;
    width: 100px;
    font-size: 10px;
}
.image
{
    width: 100px;
    height: 100px;
}

</style>