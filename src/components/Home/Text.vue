<script>
export default {

}
</script>

<template>
  <div h-100vh relative>
    <div
      py-2 w-full bg-blue absolute
      top-0 left-0 pl-30 pr-30
      inline-block flex justify-between items-center
    >
      <a href=""><div font-black text-5xl>logo</div></a>
      <div space-x-8 color-gray-1 text-2xl>
        <a href="">首页</a>
        <a href="">案例</a>
        <a href="">推荐</a>
        <a href="">个人首页</a>
      </div>
    </div>
    <div flex gap-20 items-center justify-center pt-30>
      <div
        w-120 h-180 bg-gray-100 bg-op-80 rounded-md shadow-md hover:shadow-xl transition-all
        duration-200 hover:bg-gray-100 hover:bg-op-100
      >
        test
      </div>
      <div
        w-120 h-180 bg-gray-100 bg-op-80 rounded-md shadow-md hover:shadow-xl transition-all duration-200 hover:bg-gray-100
        hover:bg-op-100
      >
        test
      </div>
    </div>
  </div>
</template>

<style>

</style>
