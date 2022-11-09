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
                    <h2>DC COMICS</h2>
                    <li>Characters</li>
                    <li>Comics</li>
                    <li>Movies</li>
                    <li>TV</li>
                    <li>Games</li>
                    <li>Videos</li>
                    <li>News</li>
                </ul>
                <ul>
                    <h2>SHOP</h2>
                    <li>Shop DC</li>
                    <li>Shop DC Collectibles</li>
                </ul>
            </div>
            <div>
                <ul>
                    <h2>DC</h2>
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
                    <h2>SITES</h2>
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
        background-position: right;
        padding: 20px 0;
        justify-content: flex-start;
        div{
            
            ul{
                list-style-type: none;
                color:white;
                margin: 20px 20px 20px 0;

                h2{
                    margin-bottom: 10px;
                    margin-right: 10px;
                }

                li{
                    color: #959595;
                    font-size: .8rem;
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