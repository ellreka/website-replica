<template>
  <nuxt-link to="#">
    <slot />
  </nuxt-link>
</template>

<style lang="scss" scoped>
a {
  display: inline-block;
  padding: 10px;
  background-color: #ff5a5f;
  border-radius: 5px;
  color: #fff;
  width: 100%;
  text-align: center;
}
</style>
