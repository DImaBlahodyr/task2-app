<template>
  <div>
    <raspberry-card
      v-for="raspberry in raspberryDataList"
      :key="raspberry.id"
      :data-raspberry="raspberry"
    />
  </div>
</template>

<script>
import RaspberryCard from './RaspberryCard.vue'

export default {
  name: 'RaspberryPanel',

  components: {
    RaspberryCard,
  },

  props: {
    raspberryDataList: {
      type: Array,
      default: () => [],
    },
  },
}
</script>

<style lang="css" scoped></style>
