<script setup>
  import DestinationCard from '@/components/DestinationCard.vue';
  import data from '@/assets/data.json'

  const destinations = data.destinations
</script>


<template>
  <h1>Home</h1>

  <div id="destinations">
    <DestinationCard v-for="(d, index) in destinations" :key="index" :dest="d"></DestinationCard>
  </div>
</template>


<style scoped>
img {
  max-width: 230px;
}
#destinations {
  display: flex;
  justify-content: space-between;
}
</style>
