<template>
  <div class="column" :justify-end="justifyEnd" :flex-start="flexStart" :justify-content="JustifyContent">
    <slot/>
  </div>
</template>
<script>
export default {
  name: 'columnComponent',
  props: {
    justifyEnd: Boolean,
    flexStart: Boolean,
    JustifyContent: Boolean
  }
}
</script>
<style>
  .column {
    display: flex;
    flex-direction: column;}
  .column[justify-content] {
    justify-content: space-between;
    text-align: left;
  }
  .column[justify-end] {
    justify-content: flex-end;
    text-align: left;
  }
  .column[flex-start] {
    justify-content: flex-start;
  }
</style>
