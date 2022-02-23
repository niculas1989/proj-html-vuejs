<template>
  <div>
    <div v-for="(t, i) in title" :key="i">
      <span class="over-the-title">{{ t.upper }}</span>
      <h2 class="fw-bolder">
        <span class="bck-prim">{{ t.bckTitle }}</span> {{ t.restOfTitle }}
      </h2>
      <span>{{ t.paragraph }}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "TitleCard",
  props: ["title"],
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_vars.scss";

.bck-prim {
  color: $prim_color;
  height: 20px;
  width: 30px;
  background-color: #daeced;
  border-radius: 3px;
}

.over-the-title {
  color: $water_green;
  font-weight: 800;
  font-size: 0.8rem;
}
</style>