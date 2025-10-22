<template>
  <div class="header">
    <div class="header-mobile">
      <div class="header-mobile__back">
        <q-icon name="arrow_back" style="color: #ccc; font-size: 2em;"></q-icon>
      </div>
      <div class="header-mobile__search">
        <q-icon name="search" style="color: #ccc; font-size: 1.6em;"></q-icon>
        <input name="search" class="header-mobile__input" standout type="text" placeholder="Поиск по сайту">
      </div>
      <div class="header-mobile__notification">
        <q-icon name="notifications_none" style="color: #ccc; font-size: 2em;"></q-icon>
      </div>
    </div>
  </div>
<Footer></Footer>
<MobileFooterMenu></MobileFooterMenu>
</template>

<script setup>
import Footer from './components/Footer.vue';
import MobileFooterMenu from './components/MobileFooterMenu.vue';

//
</script>

<style scoped lang="scss">
.header {
  min-height: 60px;
  box-shadow: 0 1px 4px #00000029;
}

.header-mobile {

  min-height: 60px;
  padding: 12px 16px;
  gap: 8px;
  display: flex;
  flex-direction: row;
  align-items: center;

  &__back {
    width: 36px;
    height: 36px;
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 8px;
    background-color: #f7f7f7;
    flex-shrink: 0;
  }

  &__search {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    height: 36px;
    padding: 0px 8px 0px 8px;
    border-radius: 8px;
    background-color: #f7f7f7;
    font-size: larger;
  }

  &__input {
    width: 100%;
    padding: 0px 8px 0px 8px;
    height: 36px;
    border-style: none;
    background-color: transparent;
  }

  &__notification {
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 8px;
    background-color: #f7f7f7;
    width: 36px;
    height: 36px;
    flex-shrink: 0;
  }
}

.v-main {
  background-color: rgb(246, 246, 246);
}
</style>
