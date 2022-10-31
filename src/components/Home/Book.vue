<script>
export default {
  data() {
    return {
      var: [1, 2, 3, 5],
    }
  },
}
</script>

<template>
  <div class="bg-[#F1FFE5]" h-100vh>
    <div h-8rem text-4xl text-center flex items-center justify-center>
      <p>书籍推荐</p>
    </div>
    <div h-40rem flex justify-center>
      <div
        p-l-40 p-t-20
        h-40rem m-auto
        overflow-x-scroll whitespace-nowrap
      >
        <div
          v-for=" item in var" :key="item" s
          m-l--10 p-l-4 class="bg-[#FDF7D2]"
          w-20rem h-28rem rounded-12 shadow-xl
          inline-block hover:-translate-y-10 hover:rotate-9 hover:w-30em transition-all
          duration-300
        >
          这是书
        </div>
      </div>
    </div>
  </div>
</template>

<style>
::-webkit-scrollbar {
  display: none; /* Chrome Safari */
}
</style>
