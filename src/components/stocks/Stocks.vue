<template>
    <div>
        <stock v-for="stock in stocks" :stock="stock"></stock>
    </div>
</template>

<script>
    import stock from "./Stock.vue";

    export default {
        data () {
            return {
                stocks: [
                    { id: 1, name: 'BMW', price: 110 },
                    { id: 2, name: 'Google', price: 200 },
                    { id: 3, name: 'Apple', price: 120 },
                    { id: 4, name: 'Twitter', price: 11 }
                ]
            }
        },
        components: {
            stock
        }
    }
</script>