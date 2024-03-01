<template>
  <div>
    <slot
      name="test"
      :data="slotProps"
    />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'SlotTest',

  data () {
    return {
      slotProps: 'Slot example'
    }
  }
})
</script>
