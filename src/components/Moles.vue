<template>
  <div class="moles-container">
    <div 
      class="mole" v-for="(moleState, index) in moleData" v-bind:key="index">
      <Mole v-bind:state="moleState" />
    </div>
  </div>
</template>

<script>
import Mole from './Mole';

export default {
  name: 'Moles',
  components: {
    Mole
  },
  props: ['moleData']
}
</script>

<style>

</style>