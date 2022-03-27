<template>
  <div class="card">
    <div class="card-image">
      <slot name="image"></slot>
    </div>
    <div class="card-header">
      <div class="card-title">
        <slot name="title"></slot>
      </div>
      <div class="card-subtitle">
        <slot name="subtitle"></slot>
      </div>
    </div>
    <div class="card-body">
      <slot name="body"></slot>
    </div>
    <div class="card-footer">
      <slot name="button"></slot>
    </div>
  </div>
</template>
<style scoped>
 .card{
   border: 1px solid black;
   width: 300px;
   height: 500px;
 }
</style>