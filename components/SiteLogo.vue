<template>
  <div class="logo-wrapper">
    <div
      :class="{
        'logo-inner': true,
      }"
    >
      <img src="/logo-frames/greenapplogo.jpeg"/>
    </div>
  </div>
</template>
<style lang="scss">
.logo-wrapper {
  position: relative;
  height: 50px;
  overflow: hidden;
  width: 200px;
  .logo-inner {
    position: absolute;
    height: 500px;
    img {
      display: block;
      height: 40px;
      margin: 5px;
      max-height: initial;
    }
  }
}
</style>
