<script>
export default {
  data() {
    return {
      cartoon: [{
        content: 'https://p1.ssl.qhimgs1.com/sdr/_240_/t01c166f44788d458f1.jpg',
      },
      {

        content: 'https://p1.ssl.qhimgs1.com/sdr/_240_/t01c166f44788d458f1.jpg',
      },
      {

        content: 'https://p1.ssl.qhimgs1.com/sdr/_240_/t01c166f44788d458f1.jpg',
      },
      {

        content: 'https://p1.ssl.qhimgs1.com/sdr/_240_/t01c166f44788d458f1.jpg',
      }],
    }
  },

}
</script>

<template>
  <div h-100vh w-full>
    <div p-15 gap-12>
      <div v-for="item in cartoon" :key="item.content" h-22rem w-40rem inline-block bg-blue m-6>
        <img :src=" item.content " h-full w-full>
      </div>
    </div>
  </div>
</template>

<style>

</style>
