<!-- AdminLayout.vue -->
<template>
  <div id="admin-layout" class="min-h-screen bg-system-gray-10">
    <!-- Sidebar -->
    <UIHeaderAdmin />
    <!-- Nội dung chính -->
    <div class="flex flex-col">
      <!-- Breadcrumb -->
      <UIBreadcrumd class="sticky top-0 z-10 bg-white/95 backdrop-blur-sm" />

      <!-- Nội dung động từ page -->
      <main class="flex-1 p-6">
        <slot />
      </main>

      <!-- Footer -->
      <PageAdminFooter />
    </div>
  </div>
</template>

<script lang="ts" setup></script>

<style lang="scss" scoped>
#admin-layout {
  @apply relative;
}
</style>
