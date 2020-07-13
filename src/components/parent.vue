<template>
<div><hr />
  <h2>Component Props in Vue.js </h2>
  <children :myProp="preciousThing"></children>
</div>
</template>

<script>
import children from './children.vue'

export default {
  components: {
    children
  },

  data () {
    return {
      preciousThing: 'ring or gold'
    }
  }
}
</script>
