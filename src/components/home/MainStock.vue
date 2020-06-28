<template>
  <div class="main-stock">
    <div class="main-img">
      <img src="../../assets/img/home/main-bg.png" alt="" />
    </div>
    <div class="main-sale">
      <div class="main-sale__title">Акция!</div>
      <div class="main-sale__description">
        При покупке климатической камеры КТХ-80 в подарок ноутбук
      </div>
      <a href="#" class="main-sale__link">Подробнее</a>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Stock',
}
</script>

<style scoped lang="scss">
.main-stock {
  position: relative;
  min-width: 400px;
  background: #3c4762 url('../../assets/img/home/el-pribor-bg.png') center
    no-repeat;
  max-height: 920px;
}
.main-img {
  position: absolute;
  top: 30px;
  left: -150px;
  right: 0;
  img {
    max-width: 600px;
  }
}

.main-sale {
  text-align: center;
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  position: absolute;
  top: 500px;
  left: 150px;
  height: 200px;
  width: 200px;
  background: rgba(60, 71, 98, 0.7);
  border-radius: 50%;
  color: #fff;
  &__title {
    font-weight: bold;
    font-size: 20px;
    margin-bottom: 25px;
  }
  &__description {
    font-weight: 500;
    font-size: 14px;
    margin-bottom: 25px;
    max-width: 180px;
  }
  &__link {
    font-weight: 500;
    font-size: 12px;
    color: #fff;
  }
}
</style>
