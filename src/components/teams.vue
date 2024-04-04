<script setup></script>

<template>
  <div class="teams__container">
    <div class="teams__block">
      <div class="teams__block__title"><b>Наши юристы</b></div>
      <div class="teams__block__text">
        <p>
          Давно выяснено, что при оценке дизайна и композиции читаемый текст мешает сосредоточиться.
          Lorem Ipsum используют потому, что тот обеспечивает более или менее стандартное заполнение
          шаблона
        </p>
      </div>
      <div class="teams__block__cards">
        <div class="card">
          <div class="card__bg"></div>
          <div class="card__info">
            <div class="card__info__name"><b>Шестакова Елизавета Егоровна</b></div>
            <div class="card__info__title"><p>Юридический консультант</p></div>
            <div class="card__info__text">
              <p>
                Есть много вариантов Lorem Ipsum, но большинство из них имеет не всегда приемлемые
                модификации, например, юмористические вставки или слова, которые даже отдалённо не
                напоминают латынь.
              </p>
            </div>
            <div class="card__info__footer"><b>12 лет юридической практики</b></div>
          </div>
          <div class="card__img"><img src="/cardimg.png" alt="cardimg" /></div>
          <div class="card__title"><b>Горюнова Полина Алексеевна</b></div>
          <div class="card__text"><p>Юрист международного права</p></div>
        </div>

        <div class="card">
          <div class="card__bg"></div>
          <div class="card__info">
            <div class="card__info__name"><b>Шестакова Елизавета Егоровна</b></div>
            <div class="card__info__title"><p>Юридический консультант</p></div>
            <div class="card__info__text">
              <p>
                Есть много вариантов Lorem Ipsum, но большинство из них имеет не всегда приемлемые
                модификации, например, юмористические вставки или слова, которые даже отдалённо не
                напоминают латынь.
              </p>
            </div>
            <div class="card__info__footer"><b>12 лет юридической практики</b></div>
          </div>
          <div class="card__img"><img src="/cardimg2.png" alt="cardimg" /></div>
          <div class="card__title"><b>Горюнова Полина Алексеевна</b></div>
          <div class="card__text"><p>Юрист международного права</p></div>
        </div>

        <div class="card">
          <div class="card__bg"></div>
          <div class="card__info">
            <div class="card__info__name"><b>Шестакова Елизавета Егоровна</b></div>
            <div class="card__info__title"><p>Юридический консультант</p></div>
            <div class="card__info__text">
              <p>
                Есть много вариантов Lorem Ipsum, но большинство из них имеет не всегда приемлемые
                модификации, например, юмористические вставки или слова, которые даже отдалённо не
                напоминают латынь.
              </p>
            </div>
            <div class="card__info__footer"><b>12 лет юридической практики</b></div>
          </div>
          <div class="card__img"><img src="/cardimg3.png" alt="cardimg" /></div>
          <div class="card__title"><b>Горюнова Полина Алексеевна</b></div>
          <div class="card__text"><p>Юрист международного права</p></div>
        </div>

        <div class="card">
          <div class="card__bg"></div>
          <div class="card__info">
            <div class="card__info__name"><b>Шестакова Елизавета Егоровна</b></div>
            <div class="card__info__title"><p>Юридический консультант</p></div>
            <div class="card__info__text">
              <p>
                Есть много вариантов Lorem Ipsum, но большинство из них имеет не всегда приемлемые
                модификации, например, юмористические вставки или слова, которые даже отдалённо не
                напоминают латынь.
              </p>
            </div>
            <div class="card__info__footer"><b>12 лет юридической практики</b></div>
          </div>
          <div class="card__img"><img src="/cardimg4.png" alt="cardimg" /></div>
          <div class="card__title"><b>Горюнова Полина Алексеевна</b></div>
          <div class="card__text"><p>Юрист международного права</p></div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.teams__container {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 80px 0px;
  background: rgb(247, 247, 247);
}
.teams__block {
  display: flex;
  flex-direction: column;
  row-gap: 50px;
  text-align: center;
}
.teams__block__title {
  display: flex;
  align-items: center;
  justify-content: center;
  color: rgb(34, 34, 34);
  font-size: 28px;
  text-transform: uppercase;
}
.teams__block__title b {
  position: relative;
  display: flex;
}

.teams__block__title b::after {
  content: '';
  position: absolute;
  display: flex;
  left: 90px;
  bottom: -15px;
  width: 25%;
  height: 3px;
  background: rgb(79, 143, 240);
}

.teams__block__text {
  font-size: 16px;
  display: flex;
  justify-content: center;
}
.teams__block__text p {
 max-width: 1100px;
}
.teams__block__cards {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 24px;
  width: 100%;
}
.card {
  position: relative;
  box-shadow: 2px 2px 12px 0px rgba(33, 33, 33, 0.12);
  background: rgb(255, 255, 255);
  cursor: pointer;
}
.card__bg {
  position: absolute;
  background: url('/border2.png') no-repeat;
  left: 25px;
  right: 0;
  top: 20px;
  bottom: 0;
  z-index: 2;
  transform: scale(1.1);
  transition: 0.4s;
  opacity: 0;
}
.card__info {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  position: absolute;
  padding: 80px 0px;
  left: 0;
  right: 0;
  top: 0;
  bottom: 0;
  background-color: #fff;
  opacity: 0;
  transition: 0.4s;
}
.card:hover .card__info {
  opacity: 1;
}
.card:hover .card__bg {
  opacity: 1;
  transform: scale(1);
}
.card__info__name {
  font-size: 16px;
}
.card__info__title {
  font-size: 14px;
}
.card__info__text {
  font-size: 14px;
}
.card__info__footer {
  font-size: 16px;
}

.card__title {
  padding: 15px 18px;
  font-size: 16px;
}
.card__text {
  padding: 0px 18px;
  margin-bottom: 20px;
  color: rgb(34, 34, 34);
  font-size: 14px;
}


</style>
