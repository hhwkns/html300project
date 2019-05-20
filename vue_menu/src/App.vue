<template>
  <div id="app">
    <ul>
      <li v-for="link in
      links"> {{link}}</li>
    </ul>
    <div class=background><h1>Carta</h1></div>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit,
      sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
      <ul class="accordian">
        <li v-for="item in menu">
          {{item.name}}
          {{item.title}}
          {{item.blurb}}
        </li>
      </ul>
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
menu:[
  {name: 'Desayuno', title: 'Comida 1', blurb: 'Lorem ipsum dolor sit amet consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'},
  {name: 'Almuerzo', title: 'Comida 2', blurb: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'},
  {name: 'Cena', title: 'Comida 3', blurb: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'}
  ],
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

h1, h2 {
  font-weight: normal;
  font-size: 5em;
}

ul, .footer {
  list-style-type: none;
  padding: 1rem;
    background-color: #ACD143;
}

.accordian {
    background-color: #FFFFFF;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}

p {
  justify: center;
}


</style>
