<template>
    <header>
        <h1>Lenox Beauty Supply</h1>
    </header>
</template>

<script>
    export default{
        name: 'MyHeader'
    };
</script>

<style scoped>
       header {
    display: flex;
    align-items: center;
    justify-content: space-between; /* To move the cart icon to the far right */
    padding: 20px 0;
}

h1 {
    text-align: center; /* To center the h1 element */
    flex: 1; /* To make sure it takes up available space */
}

.icon-cart {
    position: relative;
    margin-right: 20px;
}

.icon-cart svg {
    width: 30px;
}

.icon-cart span {
    position: absolute;
    background-color: red;
    width: 30px;
    height: 30px;
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 50%;
    color: #fff;
    top: 50%;
    right: -20px;
}
</style>