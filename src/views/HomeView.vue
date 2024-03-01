<template>
  <div>
    <img
      alt="Vue logo"
      src="../assets/logo.png"
    >
    <HelloWorld :msg="message" />
    <button @click="onClick">
      Click
    </button>

    <h2>Examples</h2>
    <div>
      <SlotsExample />
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import HelloWorld from '@/components/HelloWorld.vue'
import SlotsExample from '@/components/incompatible/SlotsExample.vue'

type Data = {
  message: string
}

export default defineComponent({
  name: 'HomeView',

  components: {
    HelloWorld,
    SlotsExample
  },

  data (): Data {
    return {
      message: 'Test @vue/compat'
    }
  },

  methods: {
    onClick (): void {
      console.log('clicked')
    }
  }
})
</script>
