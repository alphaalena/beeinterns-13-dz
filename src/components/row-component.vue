<template>
  <div class="row" :justify-start="justifyStart" :justify-center="justifyCenter">
    <slot/>
  </div>
</template>
<script>
export default {
  name: 'rowComponent',
  props: {
    justifyStart: Boolean,
    justifyCenter: Boolean
  }
}
</script>
<style>
  .row {
    justify-content: space-between;
    text-align: left;
    display: flex;
    flex-direction: row;
  }
  .row[justify-start] {
  justify-content: flex-start;
  }
  .row[justify-center] {
    justify-content: center;
  }
</style>
