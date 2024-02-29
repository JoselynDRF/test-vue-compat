<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
    <HelloWorld :msg="message" />
    <button @click="onClick">Click</button>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import HelloWorld from '@/components/HelloWorld.vue'

type Data = {
  message: string
};

export default Vue.extend({
  name: 'HomeView',

  components: {
    HelloWorld
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
