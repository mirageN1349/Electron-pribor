<template>
  <div class="main-content">
    <header class="header">
      <div class="header-block">
        <div class="header-block__logo">
          <img src="../../assets/img/home/logo.svg" alt="" />
        </div>
        <h2 class="header-block__title">
          Электрон
          <br />
          Прибор
        </h2>
      </div>

      <div class="header-block">
        <div class="header-contacts">
          <div class="header-block__contact">8 (812) - 677 - 38 - 76</div>
          <div class="header-block__info">
            <img src="../../assets/img/home/clock.svg" alt="" />
            <small>пн-пт 9:00 - 18:00</small>
          </div>
        </div>
      </div>

      <div class="header-block">
        <button class="header-block__button">Заказать звонок</button>
      </div>
    </header>

    <div class="header-info">
      <div class="header-bg">
        <img src="../../assets/img/home/header-bg.png" alt="" />
      </div>
      <h1 class="header-title">
        Климатическое оборудование
        <br />
        для предприятий
      </h1>
      <div class="header-description">
        Производство высокоточного климатического оборудования: климатические
        камеры и сушильные шкафы. Возможность производства нестандартного
        оборудования.
      </div>
      <div class="header-ui">
        <button class="header-button">
          <span>Перейти в каталог</span>
          <svg class="icon-needle">
            <use href="../../assets/img/svg/sprite.svg#needle"></use>
          </svg>
        </button>
        <div class="header-calculator">
          <div class="header-calculator__img">
            <svg class="icon-calculator">
              <use href="../../assets/img/svg/sprite.svg#calculator"></use>
            </svg>
          </div>
          <div class="header-calculator__text">Рассчитать стоимость заказа</div>
        </div>
      </div>
    </div>

    <div class="main-advantages">
      <div class="main-block">
        <div class="main-block__img">
          <img src="../../assets/img/home/diamond.svg" alt="" />
        </div>
        <div class="main-block__info">
          <h2 class="main-block__title">Серьезный опыт</h2>
          <div class="main-block__text">Более 20 лет на рынке</div>
        </div>
      </div>

      <div class="main-block">
        <div class="main-block__img">
          <img src="../../assets/img/home/like.svg" alt="" />
        </div>
        <div class="main-block__info">
          <h2 class="main-block__title">Надежность</h2>
          <div class="main-block__text">
            Поддержка заказчиков даже после истечения срока годности
          </div>
        </div>
      </div>

      <div class="main-block">
        <div class="main-block__img">
          <img src="../../assets/img/home/clock-f.svg" alt="" />
        </div>
        <div class="main-block__info">
          <h2 class="main-block__title">Большая гарантия</h2>
          <div class="main-block__text">
            Гарантия на всю продукцию 18 месяцев
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header',
}
</script>

<style scoped lang="scss">
.main-content {
  max-width: 900px;
  margin-left: 40px;
}

.header {
  display: flex;
  margin-top: 20px;
  &-title {
    margin-top: 120px;
    font-weight: bold;
    font-size: 45px;
    color: #3c4762;
  }
  &-description {
    margin-top: 40px;
    font-size: 16px;
    color: #4d4d4d;
    max-width: 650px;
  }
  &-info {
    position: relative;
  }
  &-bg {
    position: absolute;
    top: -105px;
    z-index: -1;
    opacity: 0.7;
  }
  &-ui {
    display: flex;
    margin-top: 90px;
  }
  &-button {
    outline: none;
    border: none;
    border: 1px solid transparent;
    display: flex;
    align-items: center;
    color: #fff;
    background: #3c4762;
    padding: 18px 35px 18px 35px;
    border-radius: 30px;
    font-weight: 500;
    font-size: 16px;
    font-family: 'Montserrat';
    height: 55px;
    box-shadow: 0px 15px 35px rgba(60, 71, 98, 0.44);
    transition: 0.3s;
    cursor: pointer;
    .icon-needle {
      width: 15px;
      height: 15px;
      margin-left: 15px;
      fill: white;
    }
    &:hover {
      border: 1px solid #3c4762;
      background: #fff;
      color: #3c4762;
      box-shadow: none;
      .icon-needle {
        fill: black;
      }
    }
  }
  &-calculator {
    display: flex;
    align-items: center;
    margin-left: 100px;
    .icon-calculator {
      width: 60px;
      height: 60px;
      fill: none;
      &:hover {
        fill: rgb(196, 196, 196);
        cursor: pointer;
      }
    }
    &__text {
      max-width: 210px;
      margin-left: 30px;
      color: #3c4762;
      font-weight: 500;
      font-size: 16px;
    }
  }
}

.header-block {
  display: flex;
  align-items: center;
  margin-left: 130px;
  &:first-child {
    margin-left: 0px;
  }
  &:last-child {
    margin-left: 40px;
  }
  &__logo {
    img {
      max-width: 50px;
      max-height: 50px;
    }
  }
  &__title {
    font-family: 'Alice', serif;
    font-weight: normal;
    font-size: 13px;
    text-transform: uppercase;
    color: #3c4762;
    margin-left: 20px;
  }
  &__contact {
    font-weight: 500;
    font-size: 15px;
    margin-bottom: 9px;
    font-family: 'Montserrat', 'medium';
  }
  &__info {
    display: flex;
    align-items: center;
    small {
      font-weight: 300;
      font-size: 11px;
      margin-left: 10px;
    }
  }
  &__button {
    outline: none;
    border-radius: 25px;
    border: 1px solid #3c4762;
    color: #4c4c4c;
    background: #fff;
    padding: 10px 26px;
    font-weight: 600;
    font-size: 13px;
    font-family: 'Montserrat', 'semi-bold';
    cursor: pointer;
    transition: 0.2s;
    &:hover {
      background: #747d91;
      color: #fff;
      border: 1px solid transparent;
    }
  }
}

.main-advantages {
  display: flex;
  margin-top: 90px;
}

.main-block {
  display: flex;
  flex-direction: row;
  margin-right: 30px;
  &__info {
    margin-left: 40px;
    display: flex;
    flex-direction: column;
    margin-top: 5px;
  }
  &__title {
    margin: 0;
    padding: 0;
    font-weight: bold;
    font-size: 14px;
    color: #3c4762;
  }
  &__text {
    font-weight: normal;
    font-size: 12px;
    color: #4d4d4d;
    max-width: 182px;
    margin-top: 7px;
  }
  &__img {
    display: flex;
    justify-content: center;
    min-width: 70px;
    height: 70px;
    background: #ffffff;
    box-shadow: 3px 9px 26px rgba(64, 80, 103, 0.58);
    border-radius: 50%;
  }
}
</style>
