<template>
  <a-dropdown :trigger="['click']" placement="bottomRight">
    <div :class="$style.dropdown">
      <span>EN</span>
    </div>
    <a-menu slot="overlay">
      <a-menu-item key="1">
        <span class="text-uppercase font-size-12 mr-2">EN</span>
        English
      </a-menu-item>
      <a-menu-item>
        <span class="text-uppercase font-size-12 mr-2">RU</span>
        Русский
      </a-menu-item>
      <a-menu-item>
        <span class="text-uppercase font-size-12 mr-2">CN</span>
        简体中文
      </a-menu-item>
    </a-menu>
  </a-dropdown>
</template>

<style lang="scss" module>
@import "./style.module.scss";
</style>
