<template>
<div class="app">
    <h1>Hooks as event in vue</h1>
    Hi fly! Check out the console and the code around!
    <Child @hook:mounted="childMounted"/>
    <parent />
  </div>
</template>

<script>
import parent from '@/components/parent'
import Child from './Child'
export default {
  name: 'app',
  components: { Child, parent },
  methods: {
    childMounted () {
      console.log('Child was mounted')
    }
  }
}
</script>
