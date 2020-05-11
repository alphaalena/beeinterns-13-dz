<template>
  <h1 class="heading">
    <slot/>
  </h1>
</template>
<script>
export default {
  name: 'headingComponent'
}
</script>
<style>
  .heading {
    font-weight: bold;
    font-size: 18px;
    line-height: 20px;
    text-transform: uppercase;
    color: #4A4A4A;
    text-align: left;
  }
</style>
