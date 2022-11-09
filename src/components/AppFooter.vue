<script>
export default{
    name:"AppFooter"
}
</script>

<template>
    <div class="container">
        <div class="wrapper">
            <div>
                <ul>
                    <h3>DC COMICS</h3>
                    <li>Characters</li>
                    <li>Comics</li>
                    <li>Movies</li>
                    <li>TV</li>
                    <li>Games</li>
                    <li>Videos</li>
                    <li>News</li>
                </ul>
                <ul>
                    <h3>SHOP</h3>
                    <li>Shop DC</li>
                    <li>Shop DC Collectibles</li>
                </ul>
            </div>
            <div>
                <ul>
                    <h3>DC</h3>
                    <li>prova</li>
                    <li>prova</li>
                    <li>prova</li>
                    <li>prova</li>
                    <li>prova</li>
                    <li>prova</li>
                    <li>prova</li>
                    <li>prova</li>
                    <li>prova</li>
                    <li>prova</li>
                    <li>prova</li>
                </ul>
            </div>
            <div>
                <ul>
                    <h3>SITES</h3>
                    <li>prova</li>
                    <li>prova</li>
                    <li>prova</li>
                    <li>prova</li>
                    <li>prova</li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.container{
    background-image: url(../assets/img/footer-bg.jpg);
    .wrapper{
        background-image: url(../assets/img/dc-logo-bg.png);
        background-repeat: no-repeat;
        background-position: center;
        padding: 20px;
        div{
            ul{
                list-style-type: none;
                color:white;
                margin: 20px;

                li{
                    color: #959595;
                    font-size: .7rem;
                    cursor: pointer;
                    transition: .2s;

                    &:hover{
                        color: white;
                    }
                }
            }
        }
    }
}
</style>