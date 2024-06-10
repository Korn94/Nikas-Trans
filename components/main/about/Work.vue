<template>
  <h2>Как мы работаем?</h2>
  <div class="contant">
    <img src="/assets/svg/line-small.svg" alt="SVG фоновая линия">
    <div class="box">
      <p class="title">Мы организовываем доставку груза лучшим маршрутом и в нужные сроки</p>
      <UIButton color="yellow" title="Расчитать стоимость" />
    </div>
    <div class="box">
      <div class="wrap">
        <p class="number">1</p>
        <p class="text">Вы оставляете заявку, а мы связавшись с Вами обсудим детали поставки и стоимость.</p>
      </div>
      <div class="wrap" style="margin-bottom: unset;">
        <p class="number">2</p>
        <p class="text">Ваш груз надежно упаковывается и маркируется.</p>
      </div>
      <div class="wrap" style="padding-left: 5em;">
        <ul>
          <li>подбирается транспортное средство, отвечающего международным стандартам качества на рынке перевозок.</li>
          <li>определяется оптимальный маршрут следования груза.</li>
          <li>рассчитывается стоимости перевозки груза, с учетом габарита, стоимости, характера груза, и маршрута следования.</li>
        </ul>
      </div>
      <div class="wrap">
        <p class="number">3</p>
        <p class="text">С учетом всех ваших пожеланий нами:</p>
      </div>
      <div class="wrap">
        <p class="number">4</p>
        <p class="text">Груз безопасно транспортируется до точки выгрузки и учетом правил пунктуальности международных грузоперевозок.</p>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.contant {
  position: relative;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 4em;

  .box {
    .title {
      max-width: 300px;
      font-size: 1.5em;
      margin-bottom: 3em;
    }

    .wrap {
      display: flex;
      max-width: 500px;
      align-items: center;
      margin-bottom: 1em;

      p {
        font-size: 18px;
      }

      li {
        list-style: disc;
        margin-bottom: 5px;
      }

      .number {
        font-size: 50px;
        font-weight: 600;
        color: $yellow;
        padding-right: .5em;
      }
    }
  }

  img {
    position: absolute;
    left: 14em;
    top: 8em;
  }
}

@media screen and (max-width: 860px) {
  .contant {
    flex-direction: column-reverse;

    .box .title {
      margin-top: 2em;
    }

    img {
      width: 90%;
      height: 90%;
      left: 1em;
      right: 1em;
      top: 0;
    }
  }
}

@media screen and (max-width: 460px) {
  ul {
    margin-top: 1em;
  }
}
</style>