<template>
    <div class="info">
        <div v-for="(image,index) in  imageUris" :key="index" class="image">
            <img :src="require(`../assets/images/${image.file}`)" :alt="image.text">
            <h6>{{image.text}}</h6>
        </div>
        
        
    </div>
</template>

<script>
export default {
    name:'Info',
     data() {
        return {
            imageUris:[
                {file:'buy-comics-digital-comics.png',text:'DIGITAL COMICS'},
                {file:'buy-comics-merchandise.png',text:'DC MERCHANDISE'},
                {file:'buy-comics-subscriptions.png',text:'SUBSCRIPTION'},
                {file:'buy-comics-shop-locator.png',text:'COMIC SHOP LOCATOR'},
                {file:'buy-dc-power-visa.svg',text:'DC POWER VISA'},
            ]
        }
    }
}
</script>

<style lang="scss" scoped>

@import "./../assets/scss/vars.scss";

.info
{
    background-color: $bg_color_info;
    height: 120px;
    display: flex;
    justify-content: space-around;
    align-items: center;
    color: white;

    .image{
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .image img{
        transform: scale(0.5);
    }
   
}

</style>