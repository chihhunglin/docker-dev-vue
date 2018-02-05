<template>
  <div class="counter">
    <h2>Count: {{ $store.state.count }}</h2>
    <button @click="increment">+1</button>
    <button @click="decrement">-1</button>
  </div>
</template>

<script>
import { mapActions } from 'vuex'

export default {
  methods: mapActions([
    'increment',
    'decrement'
  ])
}
</script>
