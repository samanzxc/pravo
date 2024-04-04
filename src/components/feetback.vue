<script setup>
import { ref } from 'vue'

let index = 1

function slideRight() {
  const slide = document.querySelectorAll('.slide')
  if (index > 3) {
    index = 0
  }
  index++

  slide.forEach((el) => {
    if (index === 1) {
      el.style.left = '0' + 'px'
    }
    if (index === 2) {
      el.style.left = -'24' + '%'
    }
    if (index === 3) {
      el.style.left = -'75' + '%'
    }
    if (index === 4) {
      el.style.left = -'103' + '%'
    }
  })
}
function slideLeft() {
  const slide = document.querySelectorAll('.slide')
  if (index < 2) {
    index = 5
  }
  index--
  slide.forEach((el) => {
    if (index === 1) {
      el.style.left = '0' + 'px'
    }
    if (index === 2) {
      el.style.left = -'24' + '%'
    }
    if (index === 3) {
      el.style.left = -'75' + '%'
    }
    if (index === 4) {
      el.style.left = -'103' + '%'
    }
  })
}
</script>

<template>
  <div class="feetback__container">
    <div class="feetback">
      <div class="feetback__title"><p>Что о нас говорят клиенты</p></div>
      <div class="slider">
        <div class="slider__btn">
          <div class="btn__left" @click="slideLeft">
            <img src="/btn-left.png" alt="left" />
          </div>
          <img class="line" src="/Line.png" alt="" />
          <div class="btn_right" @click="slideRight">
            <img src="/btn-right.png" alt="right" />
          </div>
        </div>
        <div class="hiden__slider">
          <div class="slides">
            <div class="slide">
              <div class="slide__top">
                <div class="wrapp">
                  <img src="/fbicon.png" alt="" />
                  <div class="slide__top__text">
                    <p>ООО “ИТ Консалтинг”</p>
                    <b>Логинова Анастасия</b>
                  </div>
                </div>
                <img class="dec" src="/fbimg.png" alt="" />
              </div>
              <div class="slide__bottom">
                <p>
                  Многие думают, что Lorem Ipsum - взятый с потолка псевдо-латинский набор слов, но
                  это не совсем так. Его корни уходят в один фрагмент классической латыни 45 года
                  н.э., то есть более двух тысячелетий назад. Ричард МакКлинток, профессор латыни из
                  колледжа Hampden-Sydney, штат Вирджиния, взял одно из самых странных слов ...
                </p>
              </div>
            </div>
            <div class="slide">
              <div class="slide__top">
                <div class="wrapp">
                  <img src="/fbicon2.png" alt="" />
                  <div class="slide__top__text">
                    <p>ООО “ИТ Консалтинг”</p>
                    <b>Логинова Анастасия</b>
                  </div>
                </div>
                <img class="dec" src="/fbimg.png" alt="" />
              </div>
              <div class="slide__bottom">
                <p>
                  Многие думают, что Lorem Ipsum - взятый с потолка псевдо-латинский набор слов, но
                  это не совсем так. Его корни уходят в один фрагмент классической латыни 45 года
                  н.э., то есть более двух тысячелетий назад. Ричард МакКлинток, профессор латыни из
                  колледжа Hampden-Sydney, штат Вирджиния, взял одно из самых странных слов ...
                </p>
              </div>
            </div>
          </div>
          <div class="slides">
            <div class="slide">
              <div class="slide__top">
                <div class="wrapp">
                  <img src="/fbicon.png" alt="" />
                  <div class="slide__top__text">
                    <p>ООО “ИТ Консалтинг”</p>
                    <b>Логинова Анастасия</b>
                  </div>
                </div>
                <img class="dec" src="/fbimg.png" alt="" />
              </div>
              <div class="slide__bottom">
                <p>
                  Многие думают, что Lorem Ipsum - взятый с потолка псевдо-латинский набор слов, но
                  это не совсем так. Его корни уходят в один фрагмент классической латыни 45 года
                  н.э., то есть более двух тысячелетий назад. Ричард МакКлинток, профессор латыни из
                  колледжа Hampden-Sydney, штат Вирджиния, взял одно из самых странных слов ...
                </p>
              </div>
            </div>
            <div class="slide">
              <div class="slide__top">
                <div class="wrapp">
                  <img src="/fbicon2.png" alt="" />
                  <div class="slide__top__text">
                    <p>ООО “ИТ Консалтинг”</p>
                    <b>Логинова Анастасия</b>
                  </div>
                </div>
                <img class="dec" src="/fbimg.png" alt="" />
              </div>
              <div class="slide__bottom">
                <p>
                  Многие думают, что Lorem Ipsum - взятый с потолка псевдо-латинский набор слов, но
                  это не совсем так. Его корни уходят в один фрагмент классической латыни 45 года
                  н.э., то есть более двух тысячелетий назад. Ричард МакКлинток, профессор латыни из
                  колледжа Hampden-Sydney, штат Вирджиния, взял одно из самых странных слов ...
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="feetback__btn">
        <button class="btn">Все отзывы</button>
        <button class="btn__two">Написать отзыв</button>
      </div>
    </div>
  </div>
</template>

<style scoped>
.feetback__container {
  background: url('/fonblock.png');
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 80px 0;
  overflow: hidden;
}
.feetback {
  display: flex;
  flex-direction: column;
  row-gap: 35px;
}
.feetback__title {
  font-size: 28px;
}
.feetback__title p {
  position: relative;
}
.feetback__title p::before {
  content: '';
  position: absolute;
  background-color: rgb(79, 143, 240);
  width: 70px;
  height: 3px;
  bottom: -15px;
}

.slider {
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;
  width: 1330px;
}
.slider__btn {
  position: absolute;
  right: 40px;
  top: -70px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  width: 45px;
}
.line {
  position: relative;
  left: 6px;
  top: 6px;
}
.btn__left img {
  position: absolute;
  cursor: pointer;
  z-index: 2;
}
.btn_right img {
  position: absolute;
  cursor: pointer;
  z-index: 2;
}
.hiden__slider {
  display: flex;
  column-gap: 35px;
  overflow: hidden;
}
.slides {
  display: flex;
  column-gap: 35px;
}
.slide {
  transition: 0.3s;
  position: relative;
  left: 0px;
  background-color: #fff;
  width: 648px;
  height: 244px;
  padding: 32px;
}
.slide__top {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.slide__top .dec {
  opacity: 0.2;
}
.wrapp {
  display: flex;
  align-items: center;
  column-gap: 24px;
}

.slide__bottom {
  margin: 15px 0;
  font-size: 14px;
}
.btn:hover {
  border: 1px black solid;
  color: black;
}
.btn__two:hover {
  border: 1px black solid;
  color: black;
}

@media (max-width: 1400px) {
  .slide {
    width: 450px;
    font-size: 13px;
    height: 200px;
    padding: 20px;
  }
  .slide__bottom {
    font-size: 12px;
  }
  .wrapp img{
    width: 50px;
  }
  .hiden__slider {
  width: 960px;
}
.feetback__title p{
  padding: 0 185px;
}
.slider__btn{
  right: 215px;
}
.feetback__btn{
  padding: 0 185px;
}
}
@media (max-width: 970px) {
  .slide {
    width: 280px;
    font-size: 10px;
    height: 160px;
    padding: 15px;
  }
  .dec {
    width: 30px;
  }
  .slide__bottom {
    font-size: 10px;
    margin: 0;
  }
  .wrapp img{
    width: 40px;
  }
  .hiden__slider {
  width: 630px;
}
.feetback__title p{
  padding-left: 350px;
  font-size: 15px;
}
.slider__btn{
  right: 385px;
}
.feetback__btn{
  padding-left: 350px;
}
}
@media (max-width: 680px) {
  .hiden__slider {
  width: 300px;
}
.feetback__title p{
  padding-left: 515px;
}
.feetback__btn{
  padding-left: 515px;
  
}
.feetback__btn button{
  padding: 7px 10px;
  font-size: 10px;
}
.slider__btn{
  right: 500px;
}
}
</style>
