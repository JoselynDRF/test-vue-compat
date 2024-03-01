<template>
  <SlotsTest>
    <template
      slot="test"
      slot-scope="{ data }"
    >
      <h2>Data: {{ data }}</h2>
    </template>
  </SlotsTest>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import SlotsTest from '@/components/incompatible/SlotsTest.vue'

export default defineComponent({
  name: 'SlotsExample',

  components: {
    SlotsTest
  }
})
</script>
