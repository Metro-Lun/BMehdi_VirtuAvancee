<script setup>
    defineProps(["dest"])



    
</script>


<template>
    <div class="destination">
        <h2>{{ dest.name }}</h2>
        <img :src="`/src/assets/images/${dest.image}`" />
    </div>
</template>


<style scoped>
    .destination {
        padding: 0.3rem;
        margin: 0.3rem;
        text-align: center;
        border: 1px solid #39495c;
    }
    .destination img {
        max-width: 230px;
    }
</style>