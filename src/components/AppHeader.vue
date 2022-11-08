<script>
export default{
    name:"AppHeader",
    data(){
        return{
            productList:[
                {
                    title:"CHARACTERS",
                    href:"/characters",
                },
                {
                    title:"COMICS",
                    href:"/comics",
                },
                {
                    title:"MOVIES",
                    href:"/movie",
                },
                {
                    title:"TV",
                    href:"/tv",
                },
                {
                    title:"GAMES",
                    href:"/games",
                },
                {
                    title:"COLLECTIBLES",
                    href:"/collectibles",
                },
                {
                    title:"VIDEO",
                    href:"/video",
                },
                {
                    title:"FANS",
                    href:"/fans",
                },
                {
                    title:"NEWS",
                    href:"/news",
                },
                {
                    title:"SHOP",
                    href:"/shop",
                },
            ]
        }
    }
}
</script>

<template>
    <div class="container">
        <div class="wrapper">
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="Logo DC">
            </div>
            <nav class="menu">
                <ul>
                    <li v-for="(item, index) in productList">
                        <a href="{{item.href}}">{{item.title}}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as*;
.logo
img{
        width: 70%;
    }

ul{
    display: flex;
    list-style-type: none;

}
    li{
        font-size: .8rem;
        padding: 45px 0;
        text-align: center;

    }
        a{
            text-decoration: none;
            color: black;
            padding: 40px 0px 40px 0;
            margin-right: 30px;

            &:hover{
                color: $primary-color;
                border-bottom: 5px solid $primary-color;
            }
        }

.wrapper{
    justify-content: space-between;
    align-items: center;
    margin-top: 10px;
}
</style>