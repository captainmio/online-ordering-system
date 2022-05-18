<template>
  <q-card>
    <q-card-section>
      <!-- Content of the card -->
      <slot name="body"></slot>
    </q-card-section>
  </q-card>
</template>

<script>
export default {
  name: "CardComponent",
};
</script>

<style>
</style>
