<template>
  <div 
    @touchstart="touchstart"
    @touchend="touchend"
    :class="$style.container"
    :style="{ backgroundColor: color }">
    <slot></slot>
    <div :class="$style.shade" :style="{ opacity: opacity, backgroundColor: highlightColor }"></div>
  </div>
</template>

<script>
export default {
  props: {
    highlightColor: {
      type: String,
      default: '#DEDEDE'
    }
  },
  data () {
    return {
      opacity: '0',
      color: null
    }
  },
  methods: {
    touchstart () {
      this.color = this.highlightColor
      this.opacity = '0.5'
    },
    touchend () {
      this.color = null
      this.opacity = '0'
    }
  }
}
</script>

<style module>
.container {
  position: relative;
}

.shade {
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  transition: all ease 0.2s;
}
</style>
