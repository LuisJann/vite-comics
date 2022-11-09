<script>
export default{
    name:"AppMain",
    data(){
        return{
            iconsList:[
                {
                    title:"DIGITAL COMICS",
                    img:"buy-comics-digital-comics.png",
                },
                {
                    title:"DC MERCHANDISE",
                    img:"buy-comics-merchandise.png",
                },
                {
                    title:"SUBSCRIPTION",
                    img:"buy-comics-subscriptions.png",
                },
                {
                    title:"COMIC SHOP LOCATOR",
                    img:"buy-comics-shop-locator.png",
                },
                {
                    title:"DC POWER VISA",
                    img:"buy-dc-power-visa.svg",
                },
            ]
        }
    },
    methods:{
        getImg(url){
            return new URL(url, import.meta.url).href;
        }
    }
}
</script>

<template>
    <div class="container">
        <div class="wrapper">
            <div class="card" v-for="(item, index) in iconsList">
                <img :src="getImg(`../assets/img/${item.img}`)" alt="">
                <p>{{item.title}}</p>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as*;
.container{
    background-color: $primary-color;
    padding: 30px 0;

    .wrapper{

        .card{
            width: calc(100% /5 - 50px);
            display: flex;
            justify-content: space-around;
            align-items: center;
            margin: 0 20px;

            img{
                width: 30%;
                margin-right: 10px;
            }
            
            p{
                color: white;
                padding-right: 30px;
                font-size: .7rem;
            }
        }
    }
}
</style>