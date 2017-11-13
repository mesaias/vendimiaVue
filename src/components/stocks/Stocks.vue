<template>
  <div>
    <app-stock v-for="sotck in stocks"></app-stock>
  </div>
</template>

<script>
  import Stocks from './Stock'
  
  export default {
    data() {
      return {
        stocks: [{
            id: 1,
            name: "GTX 970",
            price: 6200
          },
          {
            id: 2,
            name: "GTX 1070",
            price: 9500
          },
          {
            id: 3,
            name: "GTX 1080",
            price: 12000
          },
          {
            id: 4,
            name: "GTX 1080 TI",
            price: 18000
          }
        ]
      }
    },
    components:{
      appStock: Stock
    }
  }
</script>

