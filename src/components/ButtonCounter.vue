<template>
  <div class="container">
    <button v-on:click="countFunction">You clicked me {{ count }} times</button>
  </div>
</template>

<script>
export default {
  name: 'ButtonCounter',
  data: function() {
    return {
      count: 0,
    }
  },
  methods: {
    countFunction: function() {
      this.count++;
    },
    countByTwo: function() {
      this.count+=2;
    },
    countReverse: function() {
      this.count--;
    }
  }
}
</script>
<style scoped>
</style>