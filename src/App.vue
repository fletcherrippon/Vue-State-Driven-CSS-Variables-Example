<template>
  <div>
    <input type="text" v-model="color" />
    <div class="user-input-color">
      {{ color }}
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    color: 'white'
  })
}
</script>

<style scoped>
.user-input-color {
  background-color: v-bind(color)
}
</style>
