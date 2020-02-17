<template>
  <div id="app">
    <img src="./assets/logo.png">
    <h1>О мне</h1>
    <h2>{{ msg }}</h2>
    <p>
      Меня зовут Кирилл. Я UI/UX и веб-дизайнер, по совместительству frond-end разработчик,
      а так же motion дизайнер. Разрабатываю адаптивные сайты с удобным пользовательским интерфейсом.
      Делаю html баннеры наивысшего качества с любыми требованиями и технологиями.

      Интерес к программированию и к web-разработке появился тогда, когда браузеры не могли считывать кодировку. 
      Лет в 15 ко мне попала книга о Micromedia Flash MX, тогда я и познакомился с анимацией. В 9 классе я уже "фрилансил", 
      делая flash-баннера. Обучаясь в колледже, успешно совмещал учебу и работу. К чему я это все... Работать я люблю, 
      а особенно получать за это разумную плату. Поэтому всегда рад сотрудничать.
    </p>
    <h2>Контакты:</h2>
    <a href="mailto:mail@zuevkirill.ru">mail@zuevkirill.ru</a>
    <br>
    <p v-if="phoneVisibily">{{ phone }}</p>
      <button @click="phoneVisibily = !phoneVisibily" href="#" target="_blank">Показать телефон</button>
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      msg: 'страница Зуева Кирилла',
      phone: '+7 950 447 61 77',
      phoneVisibily: false
    }
  }
}
</script>

<style>
#app {
  font-family: Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
img{
  width: 250px;
}
h1, h2 {
  font-weight: normal;
}
p{
  font-size: 16px;
  line-height: 24px;
}
a{
  color: #037ACF;
}
</style>
