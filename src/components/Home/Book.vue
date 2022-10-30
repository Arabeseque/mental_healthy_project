<script>
export default {
  data() {
    return {
      var: ['牛逼', '更牛逼', '只在牛逼', 5, 6],
    }
  },
}
</script>

<template>
  <div h-100vh bg-bluegray rounded-10 m-10>
    <div h-3rem>
      书籍推荐
    </div>
    <div h-full flex justify-center>
      <div
        p-15
        h-40rem m-auto
        overflow-x-scroll whitespace-nowrap
      >
        <div

          v-for="(item,index) in var" :key="index"
          w-400px h-26rem rounded-12 bg-pink shadow-xl
          inline-block hover:-translate-x-8 hover:-translate-y-8 hover:w-30em hover:rotate-9 transition-all
          duration-300
        />
        {{ item }}
      </div>
      <!-- 想添加脚注 -->
      <!-- <div h-2rem left-0>
      书籍推荐
    </div> -->
    </div>
  </div>
</template>

<style>

</style>
