<script lang="ts">
export default {
  props: ['location'],
}
</script>

<template>
  <div class="place">
    <img :src="location.img" width="235" height="300" />
    <slot></slot>
    <p>{{ location.desc }}</p>
  </div>
</template>

<style lang="scss" scoped>
.place {
  display: flex;
  flex-direction: column;
  width: 280px;
  height: 400px;
  justify-content: center;
  align-items: center;
  background: white;
  border: 1px solid #ddd;
  padding: 20px 20px;
  margin: 10px;
  line-height: 1.15;
  h2 {
    margin: 0;
    text-align: center;
  }
  img {
    margin: 10px;
    align-self: center;
  }
}
</style>
