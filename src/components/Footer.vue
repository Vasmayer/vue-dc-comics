<template>
    <footer>
        <div class="top-footer">
            <div class="links">
                <div class="col">
                    <h4>DC COMICS</h4>
                    <ul>
                        <li v-for="(dcComicsFooterLink,index) in dcComicsFooterLinks" :key="index">{{dcComicsFooterLink}}</li> 
                    </ul>
                    <h4>SHOP</h4>
                    <ul>
                        <li v-for="(shopFooterLink,index) in shopFooterLinks" :key="index">{{shopFooterLink}}</li> 
                    </ul>
                </div>
                <div class="col">
                      <h4>DC</h4>
                        <ul>
                            <li v-for="(dcFooterLink,index) in dcFooterLinks" :key="index">{{dcFooterLink}}</li> 
                        </ul>
                </div>
                <div class="col">
                      <h4>SITES</h4>
                       <ul>
                          <li v-for="(sitesFooterLink,index) in sitesFooterLinks" :key="index">{{sitesFooterLink}}</li> 
                      </ul>
                </div>
            </div>
            <div class="logo">
                <img src="../assets/images/dc-logo-bg.png" alt="Logo DC Footer">
            </div>
        </div>
        <div class="bottom-footer">
            <div class="sign-up">
                <button>SIGN-UP NOW!</button>
            </div>
            <div class="follow-us">
                <h3>FOLLOW US</h3>
                <img src="../assets/images/footer-facebook.png" alt="facebook">
                <img src="../assets/images/footer-twitter.png" alt="twitter">
                <img src="../assets/images/footer-youtube.png" alt="youtube">
                <img src="../assets/images/footer-pinterest.png" alt="pinterest">
                <img src="../assets/images/footer-periscope.png" alt="periscope">
            </div>
        </div>
    </footer>
</template>

<script>
 export default{
    name:'Footer',
    data() {
        return {
            dcComicsFooterLinks:['Characters','Comics','Movies','TV','Games','Videos','News'],
            dcFooterLinks:['Term of Use','Privacy policy(New)','Add Choices','Advertising','Jobs','Subscriptions','Talent Workshops','CPSC Certificates','Ratings','Shop Help','Contact Us'],
            sitesFooterLinks:['DC','MAD Magazine','DC Kids','DC Universe','DC Power Visa'],
            shopFooterLinks:['Shop DC','Shop DC Collectibles']
        }
    }
 }
</script>

<style lang="scss" scoped>
@import "./../assets/scss/vars.scss";

footer
{
     font-family: $segoe-bold; 
}
 h4
 {
    color: white;
    padding: 10px 0;
 }
.top-footer
{
    background-image: url(../assets/images/footer-bg.jpg);
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    display: flex;
    justify-content: space-around;
    align-items: center;
    overflow: hidden;
    max-height: 350px;

    .links
    {
        display: flex;
        justify-content:center;
        width: 100%;

        .col
        {
             color: darkgray;
             padding: 20px;

             ul{
                 list-style-type: none;

                 li{
                    padding: 5px 0;   
                    font-size: 0.8rem;        
                 }
             }
        }
        
    }
    .logo
    {
        transform: scale(0.7);
    }
}

.bottom-footer
{
    height: 100px;
    background-color: $color-bottom-footer;
    display: flex;
    justify-content: space-around;
    align-items: center;

    .sign-up{

        button{
            color: white;
            background-color: $color-bottom-footer;
            font-size: 1.3rem; 
            border: 2px solid $blue;
            padding: 10px 15px;
        }
    }

    .follow-us
    {
        color: $blue;
        display:flex;
        justify-content:center;
        align-items: center;
       
       img,h3{
           margin: 0 10px;
       }
    }
}

</style>