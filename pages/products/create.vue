<template>
  <AppHeader title="Products" desc="Manage your products here" class="mb-6" />
  <CreateProducts />
</template>

<script setup lang="ts">
import type { VBreadcrumbItemProps } from "@morpheme/breadcrumbs";
import { onMounted } from "vue";

onMounted(() => {
  document.title = "Create Product";
});

definePageMeta({
  breadcrumbs: [
    {
      title: "Products",
      to: "/products",
    },
    {
      title: " Create Product",
      to: "/products/create",
    },
  ] as VBreadcrumbItemProps[],
});
</script>

<style scoped></style>
