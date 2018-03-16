<template>
  <div 
    @touchstart="touchstart"
    @touchend="touchend"
    :class="$style.container"
    :style="{ opacity: opacity }">
    <slot></slot>
  </div>
</template>

<script>
export default {
  data () {
    return {
      opacity: '1'
    }
  },
  methods: {
    touchstart () {
      this.opacity = '0.5'
    },
    touchend () {
      this.opacity = '1'
    }
  }
}
</script>

<style module>
.container {
  transition: all ease 0.2s;
}
</style>
