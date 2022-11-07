<template>
  <div>
    <div>
      <img src="@/assets/image/android-chrome-512x512.png" style="height: 200px; width: 200px" />
      <h1>{{ t('hello') }} , {{ t('welcome to') }} Event assistant</h1>
    </div>
  </div>
</template>

<script setup lang="ts">
const { t } = useI18n();

// const image = {
//   src: new URL('@/assets/image/android-chrome-512x512.png').href,
// };
</script>

<style lang="scss" scoped>
a {
  @apply text-sky-400 hover:(text-sky-600) transition-all ease-out duration-100;
}
</style>
