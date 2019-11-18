<template>
  <div class="wrapper">
    <div class="back">
      <div class="white"></div>
      <img src="~@/assets/toks.jpg" alt="electron-vue">
    </div>
    <div class="header">
      <b-container>
        <img src="~@/assets/logo.jpg" alt="" class="logo">
      </b-container>
    </div>
    <b-container>
      <b-row>
        <b-col lg="4" sm="6" cols="6">
          <b-card>
            <router-link to="/">
              <img id="pie-chart" src="~@/assets/001-pie-chart.png" alt="electron-vue" class="img-fluid">
              <h4 class="text-center">AYUDAS VISUALES</h4>
            </router-link>
          </b-card>
        </b-col>
        <b-col lg="4" sm="6" cols="6">
          <b-card>
            <router-link to="/directorio">
              <img id="directory" src="~@/assets/002-directory.png" alt="electron-vue" class="img-fluid">
              <h4 class="text-center">DIRECTORIO</h4>
            </router-link>
          </b-card>
        </b-col>
        <b-col lg="4" sm="6" cols="6">
          <b-card>
            <router-link to="/">
              <img id="question" src="~@/assets/003-question.png" alt="electron-vue" class="img-fluid">
              <h4 class="text-center help">PREGUNTAS FRECUENTES</h4>
            </router-link>
          </b-card>
        </b-col>
        <b-col lg="4" sm="6" cols="6">
          <b-card>
            <router-link to="/">
              <img id="process" src="~@/assets/004-process.png" alt="electron-vue" class="img-fluid">
              <h4 class="text-center">PROCEDIMIENTOS</h4>
            </router-link>
          </b-card>
        </b-col>
        <b-col lg="4" sm="6" cols="6">
          <b-card>
            <router-link to="/">
              <img id="calendar" src="~@/assets/005-calendar.png" alt="electron-vue" class="img-fluid">
              <h4 class="text-center">RECORDATORIOS</h4>
            </router-link>
          </b-card>
        </b-col>
        <b-col lg="4" sm="6" cols="6">
          <b-card>
            <router-link to="/">
              <img id="home" src="~@/assets/006-home.png" alt="electron-vue" class="img-fluid">
              <h4 class="text-center">UNIDADES</h4>
            </router-link>
          </b-card>
        </b-col>
      </b-row>
    </b-container>
  </div>
  <!--<div id="wrapper">
    <img id="logo" src="~@/assets/logo.png" alt="electron-vue">
    <h4 class="text-center"></h4>
    <main>
      <div class="left-side">
        <span class="title">
          Welcome to your new project!
        </span>
        <system-information></system-information>
      </div>

      <div class="right-side">
        <div class="doc">
          <div class="title">Getting Started</div>
          <p>
            electron-vue comes packed with detailed documentation that covers everything from
            internal configurations, using the project structure, building your application,
            and so much more.
          </p>
          <button @click="open('https://simulatedgreg.gitbooks.io/electron-vue/content/')">Read the Docs</button><br><br>
        </div>
        <div class="doc">
          <div class="title alt">Other Documentation</div>
          <button class="alt" @click="open('https://electron.atom.io/docs/')">Electron</button>
          <button class="alt" @click="open('https://vuejs.org/v2/guide/')">Vue.js</button>
        </div>
      </div>
    </main>
  </div>-->
</template>

<script>
  import 'bootstrap/dist/css/bootstrap.css'
  import 'bootstrap-vue/dist/bootstrap-vue.css'

  export default {
    name: 'landing-page',
    methods: {
    }
  }
</script>

<style>
.header{
  background: rgb(23, 22, 29);
  height: 60px;
  width: 100%;
  position: relative;
  margin-bottom: 30px;
}
.logo{
  margin: 8px 0;
  height: 100px;
}
a, a:hover{
  text-decoration: none;
  color: #fff;
  font-weight: bold;
}
.white{
  background: rgba(0, 0, 0, 0.4);
  position: absolute;
  width: 100%;
  height: 100%;
}
.back{
  position: fixed;
  min-width: 100%;
  min-height: 100%;
}
.back img{
  min-width: 100%;
  min-height: 100%;
}
.card{
  background: transparent;
  border: 0px solid transparent;
}
.card-body img{
  padding: 60px 60px 10px 60px;
}
h4{
  padding: 30px 0 0 0;
  height: 100px;
  font-size: 26px;
  text-shadow: 1px 1px 1px #000;
}
h4.help{
  padding: 38px 0 0 0;
  height: 100px;
  font-size: 20px;
  text-shadow: 1px 1px 1px #000;
}
@media (max-width: 980px) {
  .card-body img{padding: 30px 30px 5px 30px;}
}
@media (max-width: 640px) {
  .card-body img{ padding: 5px; }
  h4{ font-size: 14px; }
  h4.help{ font-size: 12px; }
}
</style>