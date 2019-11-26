<template>
  <div>
    <header class="st-Header">
      <nav class="st-Header_menu">
        <ul>
          <li></li>
          <li><nuxt-link to="#">概要</nuxt-link></li>
          <li><nuxt-link to="#">準備</nuxt-link></li>
          <li><nuxt-link to="#">安全</nuxt-link></li>
          <li><nuxt-link to="#">マネープラン</nuxt-link></li>
        </ul>
      </nav>
    </header>
  </div>
</template>

<style lang="scss" scoped>
div {
  height: 70px;
}
.st-Header {
  width: 100%;
  height: 70px;
  line-height: 70px;
  background-color: #fff;
  position: fixed;
  &_menu ul {
    display: flex;
  }
  &_menu li + li {
    margin-left: 20px;
  }
}
</style>
