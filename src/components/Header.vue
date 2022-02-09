<template>
    <header>
        <div class="logo">
            <img src="../assets/images/dc-logo.png" alt="Logo DC">
        </div>
        <nav>
            <ul>
                <li v-for="( menuLink, index ) in menuLinks" :key="index"><a :class="{ 'active': menuLink.isActive }" :href="menuLink.uri">{{menuLink.name}}</a></li>
            </ul>
        </nav>
    </header>
</template>

<script>
export default {
 name:'Header',
 data() {
   return {
    menuLinks:[
        {uri:'#',name:'Characters',isActive:false},
        {uri:'#',name:'Comics',isActive:true},
        {uri:'#',name:'Movies',isActive:false},
        {uri:'#',name:'Tv',isActive:false},
        {uri:'#',name:'Games',isActive:false},
        {uri:'#',name:'Collectibles',isActive:false},
        {uri:'#',name:'Videos',isActive:false},
        {uri:'#',name:'Fans',isActive:false},
        {uri:'#',name:'News',isActive:false},
        {uri:'#',name:'Shop',isActive:false}
    ]
   }
 }
}
</script>

<style lang="scss" scoped>
@import "./../assets/scss/vars.scss";

header
{
    height: 130px;
    background-color: white;
    display: flex;
    justify-content: space-around;
    align-items: center;
}
ul {

            display: flex;
            list-style-type: none;
            text-transform: uppercase;

            li
            {
                padding: 0 10px;
                font-size: 0.8rem;

                a{
                    color: #687378;
                    text-decoration: none;
                    font-weight: bold;
                    padding-bottom: 100%;
                }
            }
            
        }

.active
{
    border-bottom: 5px solid $active;
    color: $active;
}        

</style>
