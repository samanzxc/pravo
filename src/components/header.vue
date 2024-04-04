<script setup>
import { ref } from 'vue'

let isActive = ref(false)

function check() {
  isActive.value = !isActive.value
}
</script>

<template>
  <header class="header">
    <div class="header__top">
      <div class="header__top__left">
        <a href="#"
          ><img src="/phone.png" alt="" />
          <p>+7 (922) 022-94-82</p></a
        >
        <a href="#"
          ><img src="/mail.png" alt="" />
          <p>janis62@yahoo.com</p></a
        >
      </div>
      <div class="header__top__right">
        <p class="blue">Заказать звонок</p>
      </div>
    </div>
    <div class="header__nav">
      <div class="header__nav__logo">
        <p class="blue">Правозащитник</p>
        <b>Юридическая компания</b>
      </div>
      <ul class="header__navigation" :class="{active: isActive}">
        <img
          src="https://static.tildacdn.com/tild3063-6232-4632-b965-613134613966/4321.png"
          alt=""
          class="close"
          @click="check"
        />
        <li><a href="#">Услуги</a></li>
        <li><a href="#">О компании</a></li>
        <li><a href="#">Наши юристы</a></li>
        <li><a href="#">Отзывы</a></li>
        <li><a href="#">Новости</a></li>
        <li><a href="#">Контакты</a></li>
      </ul>
      <img class="header__menu__btn" src="https://www.testcitizenship.ca/img/menu.png" alt="" @click="check"/>
    </div>
    <div class="header__main">
      <div class="header__main__title">
        <p>Оказываем весь комплекс</p>
      </div>
      <div class="header__main__text">
        <p class="blue">Юридических услуг</p>
      </div>
      <div class="header__main__body">
        <p>
          Давно выяснено, что при оценке дизайна и композиции читаемый текст мешает сосредоточиться
          Lorem Ipsum используют потому, что тот обеспечивает более или менее стандартное
          заполнение.
        </p>
      </div>
      <div class="header__main__btn">
        <button class="btn">Наши услуги</button>
      </div>
    </div>
  </header>
</template>

<style scoped>
.header {
  display: flex;
  flex-direction: column;
  background: url('/fon.png') 50% / cover no-repeat;
  min-height: 100dvh;
  position: relative;
  overflow: hidden;
}
.header__top {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: rgb(1, 1, 1);
  padding: 20px 300px;
}
.header__top__left {
  display: flex;
  gap: 30px;
}
.header__top__left a {
  display: flex;
  align-items: center;
  gap: 15px;
  color: #fff;
}
.header__top__right {
  cursor: pointer;
}
.header__nav {
  background: rgba(1, 1, 1, 0.76);
  padding: 20px 300px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.header__navigation a {
  color: #fff;
  font-size: 18px;
  transition: 0.3s;
  position: relative;
}
.header__navigation a::before {
  content: '';
  transition: 0.3s;
  position: absolute;
  background-color: rgb(79, 143, 240);
  width: 0%;
  height: 1px;
  bottom: -3px;
}
.header__navigation a:hover::before {
  color: rgb(79, 143, 240);
  width: 100%;
}
.header__navigation a:hover {
  color: rgb(79, 143, 240);
}
.header__navigation {
  display: flex;
  column-gap: 30px;
  position: relative;
}
.header__nav__logo {
  color: #fff;
  display: flex;
  flex-direction: column;
}
.header__nav__logo p {
  font-weight: bold;
  font-size: 28px;
}
.header__nav__logo b {
  font-size: 20px;
}
.header__main {
  padding: 250px 350px;
  text-align: center;
  color: #fff;
  display: flex;
  flex-direction: column;
  row-gap: 20px;
}
.header__main__title {
  font-size: 30px;
}
.header__main__text {
  font-size: 56px;
}
.header__main__body {
  font-size: 20px;
}
.header__main__btn {
  display: flex;
  align-items: center;
  justify-content: center;
}
.header__menu__btn {
  width: 35px;
  display: none;
}
.close {
  width: 35px;
  transform: rotate(180deg);
  position: absolute;
  left: 50px;
  top: 50px;
  display: none;
}

@media (max-width: 1510px) {
  .header__top {
    padding: 20px 200px;
  }
  .header__nav {
    padding: 20px 200px;
  }
}
@media (max-width: 1320px) {
  .header__top {
    padding: 20px 100px;
    font-size: 15px;
  }
  .header__nav {
    padding: 20px 100px;
  }
  .header__nav__logo p {
    font-size: 18px;
  }
  .header__nav__logo b {
    font-size: 15px;
  }
  .header__navigation li a {
    font-size: 15px;
  }
  .header__main{
    padding: 250px 250px;
  }
}
@media (max-width: 970px) {
  .header__menu__btn {
    display: block;
    
  }
  .close {
    display: block;
  }
  .header__navigation {
    transition: .5s;
    flex-direction: column;
    position: fixed;
    right: -1000px;
    bottom: 0;
    top: 0;
    background-color: rgb(26, 26, 26);
    width: 350px;
    align-items: center;
    justify-content: center;
    row-gap: 50px;
    padding-bottom: 150px;
    z-index: 5;
  }
  .header__navigation li a {
    font-size: 22px;
  }
  .header__main{
    padding: 250px 150px;
  }
}
@media (max-width: 710px) {
  .header__top {
    padding: 20px 20px;
    font-size: 13px;
  }
  .header__main{
    padding: 250px 100px;
    font-size: 10px;
  }
  .header__main__text{
    font-size: 40px;
  }
  .header__main__body p {
    font-size: 17px;
  }
  .header__main__title{
    font-size: 25px;
  }
}
.active{
  right: 0;
}
</style>
