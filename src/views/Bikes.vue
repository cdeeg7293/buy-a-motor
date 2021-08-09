<template>
  <div>
      <h1>Bikes for Sale</h1>
    <b-table striped hover :items="bikes"></b-table>
  </div>
</template>

<script>
import bikes from '@/data/bikes'
export default {
  data () {
    return {
      bikes
    }
  }
}
</script>
