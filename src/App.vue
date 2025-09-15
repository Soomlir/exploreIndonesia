<script setup lang="ts">
import HeaderComponent from '@/components/HeaderComponent.vue';
import PromoComponent from '@/components/PromoComponent.vue';
import FeaturesComponent from '@/components/FeaturesComponent.vue';
import SecretsComponent from '@/components/SecretsComponent.vue';
import NatureComponent from '@/components/NatureComponent.vue';
import VideosComponent from '@/components/VideosComponent.vue';
import GalleryComponent from '@/components/GalleryComponent.vue';
</script>

<template>
  <div class="header-wrap">
    <HeaderComponent />
    <PromoComponent />
  </div>
  <FeaturesComponent />
  <SecretsComponent />
  <NatureComponent />
  <VideosComponent />
  <GalleryComponent />
</template>

<style scoped>
.header-wrap {
  background-image: url("/images/header-bg-mobile.jpg");
}
</style>
