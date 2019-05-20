<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
  </div>
</template>

<script lang="ts">
import { Component, Prop } from 'vue-property-decorator';
import HelloWorld from './HelloWorld.vue';

@Component
export default class ExtendHelloWorld extends HelloWorld {

  mounted() {
    this.msg = 'Yo!'
  }
}
</script>
