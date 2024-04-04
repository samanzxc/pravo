<template>
  <div class="about__container">
    <div class="about__block">
      <div class="about__left">
        <div class="about__title"><b>Юридическая компания</b><b class="blue">правозащитник</b></div>
        <div class="about__text">
          <p>
            Давно выяснено, что при оценке дизайна и композиции читаемый текст мешает
            сосредоточиться. Lorem Ipsum используют потому, что тот обеспечивает более или менее
            стандартное заполнение. <br />
            <br />
            Есть много вариантов Lorem Ipsum, но большинство из них имеет не всегда приемлемые
            модификации, например, юмористические вставки или слова, которые даже отдалённо не
            напоминают латынь. Если вам нужен Lorem Ipsum для серьёзного проекта, вы наверняка не
            хотите какой-нибудь шутки, скрытой в середине абзаца. <br />
            <br />
            За прошедшие годы текст Lorem Ipsum получил много версий. Некоторые версии появились по
            ошибке, некоторые - намеренно (например, юмористические варианты).
          </p>
        </div>
        <div class="about__btn">
          <button class="btn">История компании</button>
          <button class="btn__two">Сертефикаты</button>
        </div>
      </div>
      <div class="about__right">
        <img src="/aboutImg.png" alt="" />
      </div>
    </div>
  </div>
</template>

<style scoped>
.about__container {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 80px 30px;
}
.about__block {
  display: flex;
  width: 1319px;
}
.about__left {
  display: flex;
  flex-direction: column;
  row-gap: 35px;
}
.about__title {
  font-size: 28px;
  display: flex;
  column-gap: 15px;
}

.about__text {
  font-size: 16px;
  line-height: 150%;
}
.about__btn{
  display: flex;

}
.btn {
  margin: 0;
}
.btn:hover {
  background-color: transparent;
  border: 1px #38383852 solid;
  color: black;
}

@media(max-width: 1205px){
  .about__right{
    display: none;
  }
  .about__container {
  padding: 80px 200px;
}
.about__title{
  font-size: 20px;
}
}

</style>
