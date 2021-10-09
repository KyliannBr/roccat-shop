<template>
    <div class="card">
        <img :src="product" alt="img product" class="product">
        <p class="descProd">{{Description}}</p>
        <button>Acheter</button>
    </div>
</template>

<script>
export default {
    name: "CardProduct",
    props: {
        product: String,
        Description: String
    }
    
}
</script>

<style scoped>

    .card {
        width: 450px;
        height: 750px;
        background: linear-gradient(to bottom, #fff, #333);
    }

    img {
        width: 100%;
        height: 60%;
    }
</style>