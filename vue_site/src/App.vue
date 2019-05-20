<template>
  <div id="app">
  <ul>
    <li v-for="link in
    links"> {{link}}</li>
  </ul>
  <div class=background><h1>Comida Oaxacana</h1></div>
  <footer class="footer">
    <div class="footer-copyright text-center p-3">© 2019 Copyright:
      <a href="#"> Heather Dileepan</a>
   </div>
  </footer>

  </div>
</template>


<script>
export default {
name: 'app',
data () {
return {
links: ['Home', 'Menu', 'Gallery', 'About'],
  }
}
}
</script>


<style lang="css">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.background {
  background: url('./assets/lindsay-moe.jpg') center;
  background-size: cover;
  height: 100vh;
}

h1, h2 {
  font-weight: bold;
  font-size: 5em;
}

ul, .footer {
  list-style-type: none;
  padding: 1rem;
    background-color: #ACD143;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
  background-color: #ACD143;
}



</style>
