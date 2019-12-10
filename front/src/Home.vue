<template>
  <div>
    <h1>{{Balance}} ETH</h1>
  </div>
</template>

<script>
import web3 from '@/web3.js'

export default {
  data () {
    return {
      Balance: null
    }
  },
  beforeMount () {
    web3.eth.getCoinbase().then(address => {
      web3.eth.getBalance(address).then(balance => {
        this.Balance = Math.round(balance / 1e18 * 100) / 100
      })
    })
  }
}
</script>