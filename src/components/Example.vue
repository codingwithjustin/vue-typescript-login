<template>
  <div>{{ obj }}</div>
</template>

<script lang="ts">
import { defineComponent, PropType } from 'vue'

export default defineComponent({
  props: {
    obj: {
      type: Object as PropType<{ type: string; message: string }>,
      required: true
    }
  }
})
</script>
