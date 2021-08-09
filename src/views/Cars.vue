<template>
  <div>
      <h1>Cars for Sale</h1>
    <b-table striped hover :items="cars">
        <template slot="model" slot-scope="data">
            <router-link :to="`/motors/${data.value}`">
                {{ data.value }}
            </router-link>
      </template>
    </b-table>
  </div>
</template>

<script>
import cars from '@/data/cars'
export default {
  data () {
    return {
      cars
    }
  }
}
</script>
