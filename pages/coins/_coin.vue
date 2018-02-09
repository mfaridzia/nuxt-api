<template>
    <div>
        <h1> {{ name.toUpperCase() }} </h1>
        <p> Symbol : {{ coin.symbol }} </p>
        <p> Rank   : {{ coin.rank }} </p>
        <p> Price USD : {{ coin.price_usd }} </p>
    </div>
</template>

<script>
import axios from 'axios'

export default {
    async asyncData ({params}) {
        const { data } = await axios.get(`https://api.coinmarketcap.com/v1/ticker/${params.coin}/`)
        return { coin: data[0], name: params.coin }
    }
}
</script>

<style scoped>
div {
    margin-top:30px;
}
</style>

