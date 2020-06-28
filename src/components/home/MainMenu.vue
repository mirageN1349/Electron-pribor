<template>
  <div class="main-menu">
    <ul>
      <li v-for="item in menu" :key="item">
        {{ item }}
      </li>
    </ul>
    <button class="main-menu__button">Задать вопрос</button>
  </div>
</template>

<script>
export default {
  name: 'Menu',
  data: () => ({
    menu: ['О нас', 'Продукция', 'Услуги', 'Акции', 'Контакты'],
  }),
}
</script>

<style lang="scss" scoped>
.main-menu {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  background: #7f8aa1;
  width: 100%;
  max-width: 240px;
  color: #fff;
  max-height: 920px;
  ul {
    padding: 0;
    margin-top: 100px;
    margin-left: 40px;
    max-width: 100px;
    li {
      display: inline-block;
      margin-top: 50px;
      font-weight: normal;
      font-size: 18px;
      cursor: pointer;
      list-style-type: none;
      &::after {
        content: '';
        display: block;
        opacity: 0;
        width: 0;
        height: 2px;
        background: #fff;
        transition: 0.5s;
      }
      &:hover {
        &::after {
          opacity: 1;
          width: 100%;
        }
      }
    }
  }
  &__button {
    max-width: 175px;
    border: none;
    outline: none;
    border: 1px solid #fff;
    padding: 14px 35px;
    font-weight: 600;
    font-size: 13px;
    color: #fff;
    background: transparent;
    border-radius: 30px;
    margin-top: 190px;
    transition: 0.3s;
    font-family: 'Montserrat';
    margin-left: 30px;
    cursor: pointer;
    &:hover {
      background: #fff;
      color: #333;
    }
  }
}
</style>
