<template>
  <div class="container">
    <div class="img_container">
      <img :src="dataRaspberry.imgSrc" class="img" />
    </div>
    <div class="title">
      <img :src="dataRaspberry.logo" />
      <span>{{ dataRaspberry.companyTitle }}</span>
    </div>
    <div class="description">{{ dataRaspberry.description }}</div>
  </div>
</template>

<script>
export default {
  name: 'RaspberryCard',

  props: {
    dataRaspberry: {
      type: Object,
      default: () => ({}),
    },
  },
}
</script>

<style lang="css" scoped>
.container {
  display: inline-block;
  margin: 0px 20px;
  border: 2px solid black;
  border-radius: 7px;
  padding: 10px;
  width: 200px;
  height: 200px;
}
.img {
  width: 150px;
  border-radius: 7px;
}
.title img {
  margin-right: 6px;
}
</style>
