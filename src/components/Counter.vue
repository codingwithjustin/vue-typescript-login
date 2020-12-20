<template>
  <h4>{{ state.count }} x 2 = {{ getters.times2 }}</h4>
  <button class="btn btn-success block m-2" @click="inc(1)">
    Inc
  </button>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import counterStore from '@/stores/counter'

export default defineComponent({
  setup() {
    const { state, getters, inc } = counterStore
    return { state, getters, inc }
  }
})
</script>
