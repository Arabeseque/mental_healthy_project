<script setup lang='ts'>
interface SlideItem {
  img: string
  title: string
  subTitle: string
}
const props = defineProps<{
  item: SlideItem
}>()

const item = computed(() => props.item)
</script>

<template>
  <div flex justify-between h-100vh>
    <div
      class="leftZone" bg-black w-50vw
      flex items-center justify-center
    >
      <div color-white flex flex-col items-center justify-center>
        <div text-3xl leading-10 font-semibold>
          {{ item.title }}
        </div>
        <span text-4xl md:text-5xl font-semibold tracking-tight>
          {{ item.subTitle }}
        </span>
      </div>
    </div>
    <div class="rightZone" w-50vw flex items-center justify-center overflow-hidden>
      <img
        :src="item.img" alt="" class="rightImg"
        max-w-md
      >
    </div>
  </div>
</template>
