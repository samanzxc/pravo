<script setup></script>

<template>
  <footer class="footer">
    <div class="footer__top">
      <div class="footer__top__left">
        <p class="blue">Правозащитник</p>
        <p>Юридическая компания</p>
      </div>
      <div class="footer__top__right">
        <p>
          Предварительные выводы неутешительны: синтетическое тестирование, а также свежий взгляд на
          привычные вещи — безусловно открывает новые горизонты для экономической целесообразности
          принимаемых решений.
        </p>
      </div>
    </div>
    <div class="footer__main">
      <div class="footer__main__left">
        <div class="footer__main__left__col">
          <div class="footer__main__left__icon">
            <img src="/footerIcon1.png" alt="footerIcon" />
          </div>
          <div class="footer__main__left__text">
            <p>Наш адрес</p>
            <p class="text">г. Одинцово, пр. Будапештсткая, 40</p>
          </div>
        </div>

        <div class="footer__main__left__col">
          <div class="footer__main__left__icon">
            <img src="/footerIcon2.png" alt="footerIcon" />
          </div>
          <div class="footer__main__left__text">
            <p>Запись на консультанцию</p>
            <p class="text">+7 (922) 022-94-82</p>
          </div>
        </div>

        <div class="footer__main__left__col">
          <div class="footer__main__left__icon">
            <img src="/footerIcon3.png" alt="footerIcon" />
          </div>
          <div class="footer__main__left__text">
            <p>Корреспонденция</p>
            <p class="text">janis62@yahoo.com</p>
          </div>
        </div>
      </div>
      <div class="footer__main__middle">
        <ul>
          <li>Услуги</li>
          <li>О компании</li>
          <li>Сертификаты</li>
          <li>Отзывы</li>
          <li>Полезные материалы</li>
          <li>Благотворительность</li>
        </ul>
      </div>
      <div class="footer__main__right">
        <div class="footer__main__right__top">
          <div class="footer__main__right__top__icon">
            <img src="/footerMidleIcon.png" alt="footerMidleIcon" />
          </div>
          <div class="footer__main__right__top__text">
            <h3>Миронов Александр</h3>
            <p>Ведущий юрист</p>
          </div>
        </div>
        <div class="footer__main__right__text">
          <p>
            Есть над чем задуматься: тщательные исследования конкурентов разоблачены. Идейные
            соображения высшего порядка, а также перспективное планирование играет
          </p>
        </div>
        <button class="btn">Задать вопрос юристу</button>
      </div>
    </div>
  </footer>
  <div class="footer__bottom">
    <p>Все права защищены, 2023</p>
    <p>Политика обработки персональных данных</p>
  </div>
</template>

<style scoped>
.footer {
  background: rgb(34, 34, 34);
  color: #fff;
  padding: 0px 300px;
}
.footer__top {
  display: flex;
  align-items: center;
  column-gap: 25px;
  justify-content: space-between;
  border-bottom: 1px solid rgba(140, 140, 140, 0.253);
  padding: 80px 0;
}
.footer__top__left {
  display: flex;
  flex-direction: column;
  font-size: 20px;
}
.footer__top__left p {
  font-weight: bold;
}
.blue {
  color: rgb(79, 143, 240);
  font-size: 28px;
  font-weight: bold;
}
.footer__top__right {
  width: 70%;
  font-size: 16px;
}
.footer__main {
  display: flex;
  align-items: center;
  column-gap: 25px;
  justify-content: space-between;
}
.footer__main__left {
  display: flex;
  flex-direction: column;
  row-gap: 25px;
}
.footer__main__left__col {
  display: flex;
  column-gap: 25px;
}
.footer__main__left__text {
  color: #ffffff6c;
}
.text {
  color: #ffffff;
}
.footer__main__middle ul {
  display: flex;
  flex-direction: column;
  row-gap: 20px;
}
.footer__main__middle ul li:hover {
  color: rgb(79, 143, 240);
  cursor: pointer;
}
.footer__main__right {
  display: flex;
  flex-direction: column;
  row-gap: 20px;
  width: 490px;
  padding: 50px 0;
}
.footer__main__right__top {
  display: flex;
  align-items: center;
  column-gap: 20px;
}

.footer__main__right__top__text {
  font-size: 19px;
}
.footer__main__right__top__text p {
  font-size: 14px;
}

.footer__main__right__btn {
  width: 100%;
}
.btn {
  width: 50%;
}
.footer__bottom {
  background: rgb(24, 24, 24);
  color: #fff;
  display: flex;
  align-content: center;
  justify-content: space-between;
  padding: 15px 300px;
  font-size: 14px;
}

@media (max-width: 1520px) {
  .footer {
    padding: 0 150px;
  }
}
@media (max-width: 1070px) {
  .footer__top p {
    font-size: 15px;
  }
  .footer__top__right p {
    font-size: 12px;
  }
  .footer__bottom p {
    font-size: 12px;
  }
  .footer__bottom {
    padding: 15px 200px;
  }
  .btn {
    font-size: 10px;
    padding: 7px 10px;
  }
}
@media (max-width: 960px) {
  .footer__main__left img {
    width: 30px;
  }
  .footer__main__left__text{
    font-size: 12px;
  }
  .footer__main__middle ul {
    font-size: 12px;
  }
  .footer__main__right{
    font-size: 11px;
  }
  .footer__main__right__top__text{
    font-size: 11px;
  }
  .footer__main__right__top__icon img{
    width: 45px;
  }
  .footer {
    padding: 0 50px;
  }
}
@media (max-width: 640px) {
  .footer__main{
    flex-wrap: wrap;
    align-items: center;
    padding-top: 20px;
    row-gap: 20px;
  }
  .footer__main__middle{
    display: none;
  }
  .footer__bottom {
    padding: 15px 50px;
    column-gap: 10px;
  }
}
</style>
