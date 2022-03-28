<template>
  <div class="footer">
    <slot></slot>
  </div>
</template>
<style scoped>
.footer {
  width: 100%;
  height: 100px;
  line-height: 100px;
  background-color: lightgrey;
  position:fixed;
    width:100%;
    bottom:0px;
}
slot{
  display: inline-block;
}
</style>