<script setup>

</script>

<template>
<div class="blog__block">
    <div class="blog__body">
      <div class="blog__title"><b>Наши услуги</b></div>
      <div class="blog__text">
        <p>
          Давно выяснено, что при оценке дизайна и композиции читаемый текст мешает сосредоточиться.
          Lorem Ipsum используют потому, что тот обеспечивает более или менее стандартное заполнение
          шаблона
        </p>
      </div>
      <div class="blog__cards">
        <div class="card">
          <div class="card__bgh"></div>
          <div class="card__img"><img src="/blogImg.png" alt="blogImg"></div>
          <div class="card__title"><b>Воистину радостный звук: шёпот бессменных лидеров</b></div>
          <div class="card__text"><p>24 апр. 2023 г.</p><div class="card__decor"></div></div>
          <div class="card__footer"><p>Предварительные выводы неутешительны: синтетическое тестирование, а также свежий взгляд на привычные вещи — безусловно открывает новые горизонты для экономической целесообразности принимаемых решений. </p></div>
        </div>

        <div class="card">
          <div class="card__bgh"></div>
          <div class="card__img"><img class="bg" src="/blog2bg.png" alt=""><img src="/blogImg2.png" alt="blogImg"></div>
          <div class="card__title"><b>Франция намерена исследовать, почему объемы выросли</b></div>
          <div class="card__text"><p>12 апр. 2023 г.</p><div class="card__decor"></div></div>
          <div class="card__footer"><p>Для современного мира новая модель организационной деятельности влечет за собой процесс внедрения и модернизации вывода текущих активов. Являясь всего лишь частью общей картины, базовые сценарии поведения...</p></div>
        </div>

        <div class="card">
          <div class="card__bgh"></div>
          <div class="card__img"><img src="/blogImg3.png" alt="blogImg"></div>
          <div class="card__title"><b>Сплочённость команды профессионалов продолжает удивлять</b></div>
          <div class="card__text"><p>02 фев. 2023 г.</p><div class="card__decor"></div></div>
          <div class="card__footer"><p>Современные технологии достигли такого уровня, что курс на социально-ориентированный национальный проект способствует повышению качества соответствующих условий активизации. </p></div>
        </div>

      </div>
      <div class="blog__btn">
        <button class="btn">Все новости</button>
      </div>
    </div>
  </div>
</template>

<style scoped>
.blog__body {
  display: flex;
  flex-direction: column;
  text-align: center;
  gap: 30px;
  padding: 80px 150px;
}
.blog__title {
  font-size: 28px;
}
.blog__title b {
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
}
.blog__title b::before {
  content: '';
  position: absolute;
  background-color: rgb(79, 143, 240);
  width: 70px;
  height: 3px;
  bottom: -15px;
}
.blog__text {
  display: flex;
  justify-content: center;
}
.blog__text p {
  width: 900px;
}
.blog__cards {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  column-gap: 38px;
  row-gap: 30px;
}
.card {
  width: 424px;
  display: flex;
  flex-direction: column;
  row-gap: 20px;
  justify-content: space-between;
  transition: 0.3s;
  position: relative;
  cursor: pointer;
  text-align: start;
}
.card__bgh {
  background: url('/border32.png') no-repeat;
  position: absolute;
  left: 28px;
  top: 25px;
  right: 0px;
  bottom: 0px;
  transform: scale(1.1  );
  opacity: 0;
  transition: 0.4s;
  z-index: 2;
}
.card:hover .card__bgh {
  transform: scale(1);
  opacity: 1;
}
.card:hover .card__title{
    color: rgb(79, 143, 240);
}

.card__title {
  font-size: 20px;
  
}
.card__text {
  font-size: 14px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.card__decor {
    background-color: rgba(0, 0, 0, 0.082);
    height: 1px;
    width: 60%;
}
.btn:hover {
    color: #000000;
    border: 1px #00000094 solid;
}
.card__img{
  position: relative;
}
.bg {
  position: absolute;
}

@media(max-width: 525px){
  .blog__body{
    padding: 80px 50px;
  }
  .card{
    width: 350px;
  }
  .card__img img{
    width: 100%;
  }
}
</style>
