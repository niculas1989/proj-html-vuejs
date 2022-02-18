<template>
  <div>
    <div v-for="(i, index) in info" :key="index">
      <p>{{ i.open }}</p>
    </div>
  </div>
</template>

<script>
export default {
  props: ["info"],
};
</script>

<style scoped lang="scss">
</style>