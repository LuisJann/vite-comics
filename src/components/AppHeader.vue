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
        width: 50%;
        margin-right: 30px; 
    }

ul{
    display: flex;
    list-style-type: none;

}
    li{
        margin: 0px 10px;
        padding-bottom: 20px;
        font-size: .8rem;

        &:hover{
            border-bottom: 4px solid $primary-color;
        }
    }
        a{
            text-decoration: none;
            color: black;

            &:hover{
                color: $primary-color;
            }
        }

.wrapper{
    justify-content: space-between;
    align-items: center;
    margin-top: 10px;
}
</style>