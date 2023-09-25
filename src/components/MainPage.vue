<template>
  <div class="wrapper">
    <MainSearch />
    <MainCards />
    <MainPagination />
  </div>
</template>

<script setup>
  import MainSearch from '@/components/MainSearch.vue'
  import MainCards from '@/components/MainCards.vue'
  import MainPagination from '@/components/MainPagination.vue'
</script>

<style scoped lang="postcss">
  .wrapper {
    @apply container mx-auto flex flex-col gap-4 py-4;
  }
</style>
<!-- eslint-disable-next-line vue/multi-word-component-names -->
