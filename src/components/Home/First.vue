<script setup lang="ts">
const route = [
  {
    name: '首页',
    path: '/',
  },
  {
    name: '案例',
    path: '/about',
  },
  {
    name: '推荐',
    path: '/contact',
  },
  {
    name: '个人首页',
    path: '/personal',
  },
]

const router = useRouter()
const handleRoute = (path: any) => {
  router.push(path)
}
</script>

<template>
  <div h-100vh relative class="bg-[#CAEDEB]" rounded-l-xl>
    <p>test</p>
    <div
      py-2 w-full class="bg-[#CAEDEB]" absolute top-0 left-0 pl-30 pr-30 inline-block flex justify-between
      items-center
    >
      <a href="">
        <div font-black text-5xl>logo</div>
      </a>
      <div
        class="color-[#684F36]" text-2xl flex items-center justify-center gap-8
      >
        <div
          v-for="item in route"
          :key="item.name"
          cursor-pointer
          @click="handleRoute(item.path)"
        >
          {{ item.name }}
        </div>
      </div>
    </div>
    <div absolute left-30rem top-23rem>
      <div text-20 text-left>
        WelCome !
      </div>
      <p text-8 text-left>
        欢迎来到本页面！我们将会为您推荐最合理的解决方案！请向下滚动以继续！
      </p>
      <p text-left>
        Welcome to this page! We will recommend the most reasonable solution for you!
      </p>
    </div>
  </div>
</template>

<style>

</style>
