<script setup>
  import { ref } from 'vue'
  const brand = ref('🏬 Lake Company Directory')
</script>

<template>
  <nav>
    <div class="wrapper">
      <div class="brand">
        <span class="brand-title">{{ brand }}</span>
      </div>
      <div class="menu">
        <a href="#" class="menu-item">Departments</a>
        <a href="#" class="menu-item">Settings</a>
        <a href="#" class="menu-login">Logout</a>
      </div>
    </div>
  </nav>
</template>

<style scoped lang="postcss">
  nav {
    @apply flex h-20 bg-teal-700 text-slate-200;
    .wrapper {
      @apply container mx-auto flex w-full items-center justify-between;
      .brand {
        &-title {
          @apply text-3xl font-bold text-lime-300;
        }
      }
      .menu {
        @apply flex gap-2;
        &-item {
          @apply rounded-md px-4 py-2 hover:bg-purple-300 hover:text-red-700;
        }
        &-item:hover {
          @apply font-bold;
        }
        &-login {
          @apply rounded-md bg-orange-300 px-4 py-2 font-bold text-slate-800 hover:bg-purple-300;
        }
      }
    }
  }
</style>
