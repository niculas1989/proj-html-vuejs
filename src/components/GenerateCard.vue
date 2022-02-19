<template>
  <div>
    <div>
      <div class="squared">
        <img :src="e.img" :alt="e.alt" class="image-fluid" />
        <p>{{ e.title }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "GenerateCard",
  props: ["element"],
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_vars.scss";

.squared {
  height: 200px;
  width: 200px;
}
</style>