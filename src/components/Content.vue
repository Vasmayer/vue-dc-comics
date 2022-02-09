<template>
    <main>
        <div class="jumbotron">
            
        </div>
        <div class="content">
            <Cardw />
        </div>
    </main>
</template>

<script>
 import Card from './Card.vue'; 

export default {
    name:'Content',
    components: {
        Card,
  }
}
</script>

<style lang="scss" scoped>

@import "./../assets/scss/index.scss";

main
{

    .jumbotron
    {
        background-image: url(../assets/images/jumbotron.jpg);
 
        height: 350px;
    }
    .content
    {
        background-color: $color_content;
    }
}
</style>