<script setup lang='ts'>
</script>

<template>
  <div h-100vh>
    <div pt-14>
      <div text-3xl>
        文章列表
      </div>
    </div>
    <div flex justify-center items-center gap-8 pt-12>
      <div
        relative
        bg-gray-50 bg-op-60 w-20rem h-30rem shadow-md rounded-md hover:shadow-xl transtion-all duration-100
      >
        <div
          class="bottomNav"

          absolute bottom-2 flex justify-between items-center w-full p-2
        >
          <div
            class="avator"

            flex items-center justify-center gap-2
          >
            <img
              rounded-full w-8 h-8
              src="https://images.unsplash.com/photo-1666786556752-97d6e83110d3?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxlZGl0b3JpYWwtZmVlZHwzNHx8fGVufDB8fHx8&auto=format&fit=crop&w=500&q=60" alt=""
            >
            Author
          </div>
          <div
            class="readMore"

            flex items-center justify-center gap-2
            op-60
          >
            Read More
            <div i-ic:baseline-arrow-forward />
          </div>
        </div>
        <div flex flex-col items-center justify-center>
          <div text-3xl pt-7>
            Title
          </div>
          <div
            class="content"
            pt-4 px-6 overflow-hidden h-50vh text-ellipsis w-full
          >
            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Voluptate laborum dolore nulla atque, aut mollitia exercitationem quisquam suscipit earum voluptatibus distinctio repudiandae reiciendis culpa ratione a, dolores error libero esse.
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Sequi et sed accusamus. Architecto dolor aut cum repellat, harum vel deserunt praesentium eaque blanditiis ea totam veritatis consectetur excepturi quod facilis.
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Sequi et sed accusamus. Architecto dolor aut cum repellat, harum vel deserunt praesentium eaque blanditiis ea totam veritatis consectetur excepturi quod facilis.
          </div>
        </div>
      </div>
      <div
        relative
        bg-gray-50 bg-op-60 w-20rem h-30rem shadow-md rounded-md hover:shadow-xl transtion-all duration-100
      >
        <div
          class="bottomNav"

          absolute bottom-2 flex justify-between items-center w-full p-2
        >
          <div
            class="avator"

            flex items-center justify-center gap-2
          >
            <img
              rounded-full w-8 h-8
              src="https://images.unsplash.com/photo-1666786556752-97d6e83110d3?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxlZGl0b3JpYWwtZmVlZHwzNHx8fGVufDB8fHx8&auto=format&fit=crop&w=500&q=60" alt=""
            >
            Author
          </div>
          <div
            class="readMore"

            flex items-center justify-center gap-2
            op-60
          >
            Read More
            <div i-ic:baseline-arrow-forward />
          </div>
        </div>
        <div flex flex-col items-center justify-center>
          <div text-3xl pt-7>
            Title
          </div>
          <div
            class="content"
            pt-4 px-6 overflow-hidden h-50vh text-ellipsis w-full
          >
            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Voluptate laborum dolore nulla atque, aut mollitia exercitationem quisquam suscipit earum voluptatibus distinctio repudiandae reiciendis culpa ratione a, dolores error libero esse.
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Sequi et sed accusamus. Architecto dolor aut cum repellat, harum vel deserunt praesentium eaque blanditiis ea totam veritatis consectetur excepturi quod facilis.
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Sequi et sed accusamus. Architecto dolor aut cum repellat, harum vel deserunt praesentium eaque blanditiis ea totam veritatis consectetur excepturi quod facilis.
          </div>
        </div>
      </div>
      <div
        relative
        bg-gray-50 bg-op-60 w-20rem h-30rem shadow-md rounded-md hover:shadow-xl transtion-all duration-100
      >
        <div
          class="bottomNav"

          absolute bottom-2 flex justify-between items-center w-full p-2
        >
          <div
            class="avator"

            flex items-center justify-center gap-2
          >
            <img
              rounded-full w-8 h-8
              src="https://images.unsplash.com/photo-1666786556752-97d6e83110d3?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxlZGl0b3JpYWwtZmVlZHwzNHx8fGVufDB8fHx8&auto=format&fit=crop&w=500&q=60" alt=""
            >
            Author
          </div>
          <div
            class="readMore"

            flex items-center justify-center gap-2
            op-60
          >
            Read More
            <div i-ic:baseline-arrow-forward />
          </div>
        </div>
        <div flex flex-col items-center justify-center>
          <div text-3xl pt-7>
            Title
          </div>
          <div
            class="content"
            pt-4 px-6 overflow-hidden h-50vh text-ellipsis w-full
          >
            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Voluptate laborum dolore nulla atque, aut mollitia exercitationem quisquam suscipit earum voluptatibus distinctio repudiandae reiciendis culpa ratione a, dolores error libero esse.
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Sequi et sed accusamus. Architecto dolor aut cum repellat, harum vel deserunt praesentium eaque blanditiis ea totam veritatis consectetur excepturi quod facilis.
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Sequi et sed accusamus. Architecto dolor aut cum repellat, harum vel deserunt praesentium eaque blanditiis ea totam veritatis consectetur excepturi quod facilis.
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.content {
  display:-webkit-box;
  -webkit-box-orient:vertical;
  -webkit-line-clamp:13;
}
</style>

