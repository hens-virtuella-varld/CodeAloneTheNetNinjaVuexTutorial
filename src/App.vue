<template>
    <div id="app">
        <product-list-one v-bind:products="products"></product-list-one>
        <product-list-two v-bind:products="products"></product-list-two>
    </div>
</template>

<script>
import ProductListOne from "./components/ProductListOne";
import ProductListTwo from "./components/ProductListTwo";

export default {
    components: {
        "product-list-one": ProductListOne,
        "product-list-two": ProductListTwo,
    },
    name: "App",
    data() {
        return {
            products: [
                { name: "Banana Skin", price: 20 },
                { name: "Skiny Star", price: 40 },
                { name: "Green Shells", price: 60 },
                { name: "Red Shells", price: 80 },
            ],
        };
    },
};
</script>

<style>
body {
    font-family: "Ubuntu", sans-serif;
    color: #555;
}
</style>
