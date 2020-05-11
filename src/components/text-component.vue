<template>
  <p class="text" :text-opacity="textOpacity" :little="little" :little-fatty="littleFatty">
    <slot/>
  </p>
</template>
<script>
export default {
  name: 'textComponent',
  props: {
    textOpacity: Boolean,
    little: Boolean,
    littleFatty: Boolean
  }
}
</script>
<style>
  .text {
    font-size: 14px;
    line-height: 16px;
    color: #4A4A4A;
    margin-top: 0px;
    margin-bottom: 10px;
    text-align: left;
  }
  .text[text-opacity] {
    font-weight: bold;
    color: #4A4A4A;
    opacity: 0.5
  }
  .text[little]{
    font-size: 12px;
    line-height: 14px;
    color: #4A4A4A;
    margin-top: 5px;
    margin-bottom: 2px;
  }
  .text[little-fatty]{
    font-weight: bold;
    font-size: 12px;
    line-height: 14px;
    color: #4A4A4A;
  }
</style>
