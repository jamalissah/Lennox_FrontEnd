<template>
    <div class="item-box">
        <img :src="item.image" alt="item.name">
        <h2>{{  item.name  }}</h2>
        <h3>Category: {{ item.category }}</h3>
        <div class="stock"><h3>In stock: {{  item.stock }}</h3></div>
        <button class="price">${{  item.price.toFixed(2) }}</button>
    </div>
</template>

<script>
    export default{
        name: 'ItemBox',
        props: {
            item: Object
        }
    };

</script>

<style scoped>
    .item-box{
    background-color: #EEEEE6;
    padding: 20px;
    border-radius: 20px;
    }

    .item-box img{
    width: 90%;
    height: 200px;
    filter: drop-shadow(0 50px 20px #0009);
    }

    .item-box h2{
    font-weight: 500;
    font-size: large;
    }

    .item-box button{
        background-color: #353432;
        color: #eee;
        border: none;
        padding: 5px 10px;
        margin-top: 10px;
        border-radius: 20px;
        font-weight: 500;
        font-size: large;
    }
</style>