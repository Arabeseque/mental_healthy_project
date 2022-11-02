<script setup lang="ts">
import scrollIntoView from 'smooth-scroll-into-view-if-needed'
const eventHandle = {
  getEvent(event) {
    return event || window.event
  },
  addEvent(element, type, handler) {
    if (element.addEventListener)
      element.addEventListener(type, handler, false)

    else if (element.attachEvent)
      element.attachEvent(`on${type}`, handler)
    else
      element[`on${type}`] = handler
  },
  getWheelDelta(event) {
    return event.wheelDelta ? event.wheelDelta : (-event.detail) * 40
  },
}
eventHandle.addEvent(document, 'mousewheel', mouseHandle)
eventHandle.addEvent(document, 'DOMMouseScroll', mouseHandle)
function mouseHandle(event) {
  event = eventHandle.getEvent(event)
  const delta = eventHandle.getWheelDelta(event)
  const nowPos = window.scrollY
  const navPos = document.getElementById('nav').getBoundingClientRect().top + window.scrollY
  if (nowPos >= 0 && nowPos < navPos) {
    if (delta > 0) {
      console.log('video')
      scrollIntoView(document.getElementById('video'), {
        scrollMode: 'if-needed',
        block: 'nearest',
        inline: 'nearest',
      })

      console.log('up')
    }
    if (delta < 0) {
      scrollIntoView(document.getElementById('nav'), {
        scrollMode: 'if-needed',
        block: 'nearest',
        inline: 'nearest',
      })
      console.log('down')
    }
  }
}
</script>

<template>
  <div id="video">
    <Video />
  </div>
  <First id="nav" />
  <div relative>
    <div sticky h-100vh top-0 bg-blue-100>
      <!-- <Text /> -->
    </div>
    <div
      sticky h-100vh top-20 bg-black
      rounded-l-xl m-l-10
    >
      <Book />
    </div>
    <div
      sticky h-100vh top-25 bg-amber
      rounded-l-xl m-l-15
    >
      <!-- <Movie /> -->
    </div>
    <div sticky h-100vh top-30 bg-amber-100 rounded-l-xl m-l-20>
      <!-- <Movie /> -->
    </div>
    <div sticky h-100vh top-35 bg-amber-500 rounded-l-xl m-l-25 overflow-hidden relative>
      <div
        absolute
        p-r-0 rounded-xl overflow-hidden
        h-80 w-100
        duration-300 transition-all
        bg-amber-500
        class="left-[50%] top-[50%] translate-x-[-50%] translate-y-[-50%]"
        hover:w-full hover:h-full
      >
        <video
          controls
          src="../assets/share.mp4"
          loop

          muted
          w-full h-full object-cover
        />
        <!-- <Movie /> -->
      </div>
    </div>
    <div h-100vh>
      <!-- <Movie /> -->
    </div>
  </div>
</template>

<style>

</style>
