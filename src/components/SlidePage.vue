<script setup lang='ts'>
const tailContainer = $ref<HTMLElement>()

const slideItem = [
  {
    img: 'https://cdn.jsdelivr.net/gh/Arabeseque/pictureBed/202210271532352.png',
    title: 'We built',
    subTitle: 'Pink Panda App',
  },
  {
    img: 'https://cdn.jsdelivr.net/gh/Arabeseque/pictureBed/202210271532961.png',
    title: 'We built',
    subTitle: 'Pink Panda App',
  },
  {
    img: 'https://cdn.jsdelivr.net/gh/Arabeseque/pictureBed/202210271532802.png',
    title: 'We built',
    subTitle: 'Pink Panda App',
  },
]
</script>

<template>
  <div ref="tileContainer" relative>
    <div v-for="item in slideItem" :key="item.img" h-100vh sticky top-0>
      <SlideItem
        :item="item"
      />
    </div>
  </div>
</template>

<style>

</style>
