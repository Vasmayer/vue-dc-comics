<template>
    <footer>
        <div class="top-footer">
            <div class="links">
                <div class="col">
                    <h4>DC COMICS</h4>
                    <ul>
                        <li v-for="(dcComicsFooterLink,index) in dcComicsFooterLinks" :key="index">{{dcComicsFooterLink}}</li> 
                    </ul>
                </div>
                <div class="col">
                      <h4>DC</h4>
                       <ul>
                        <li>aaaaaaaaaaaaaaa</li>
                        <li>aaaaaaaaaaaaaaa</li>
                        <li>aaaaaaaaaaaaaaa</li>
                        <li>aaaaaaaaaaaaaaa</li>
                        <li>aaaaaaaaaaaaaaa</li>
                        <li>aaaaaaaaaaaaaaa</li>
                        <li>aaaaaaaaaaaaaaa</li>
                        <li>aaaaaaaaaaaaaaa</li>
                    </ul>
                </div>
                <div class="col">
                      <h4>SITES</h4>
                       <ul>
                        <li>aaaaaaaaaaaaaaa</li>
                        <li>aaaaaaaaaaaaaaa</li>
                        <li>aaaaaaaaaaaaaaa</li>
                        <li>aaaaaaaaaaaaaaa</li>
                        <li>aaaaaaaaaaaaaaa</li>
                        <li>aaaaaaaaaaaaaaa</li>
                        <li>aaaaaaaaaaaaaaa</li>
                        <li>aaaaaaaaaaaaaaa</li>
                    </ul>
                </div>
            </div>
            <div class="logo">
                <img src="../assets/images/dc-logo-bg.png" alt="Logo DC Footer">
            </div>
        </div>
        <div class="bottom-footer"></div>
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
</script>

<style lang="scss" scoped>

$segoe-bold: 'Segoe UI Bold', 'Open Sans', Helvetica, sans-serif;

 h4
 {
             color: white;
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
    font-family: $segoe-bold; 

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
        transform: scale(1.2);
    }
}

</style>