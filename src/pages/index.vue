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
  <Video id="video" />
  <!-- <Home /> -->
  <Text id="nav" />
  <Book />
  <Movie />
  <Cartoon />
  <SlidePage />
  <!-- <Footer /> -->
</template>

<style>

</style>
