<template>
    <div class="info">
        <div v-for="(imageUri,index) in  imageUris" :key="index" class="image">
            <img :src="require(`../assets/images/${imageUri}`)" alt="">
        </div>
        
    </div>
</template>

<script>
export default {
    name:'Info',
     data() {
        return {
            imageUris:['buy-comics-digital-comics.png','buy-comics-merchandise.png','buy-comics-subscriptions.png','buy-comics-shop-locator.png','buy-dc-power-visa.svg']
        }
    }
}
</script>

<style lang="scss" scoped>

$bg_color_info:#0082F9;

.info
{
    background-color: $bg_color_info;
    height: 120px;
    display: flex;
    justify-content: space-around;
    align-items: center;
    color: white;

    .image img{
        transform: scale(0.5);
    }
   
}

</style>