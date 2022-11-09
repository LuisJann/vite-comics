<script>
export default{
    name:"ContentSection",
    props:{
        img: String,
        text: String,
        price: String,
    },
}
</script>

<template>
    <div class="card">
        <img :src="img" alt="">
        <h5>{{text}}</h5>
        <p>{{price}}</p>
    </div>
</template>

<style lang="scss" scoped>
        .card{
            width: calc(100% / 6 - 20px);
            margin: 10px;
            cursor: pointer;
            transition: .2s;

            &:hover{
                transform: scale(1.1);
            }
            
            h5{
                color: white;
            }
            p{
                color: #959595;
                font-size: .7rem;
            }
        }
</style>