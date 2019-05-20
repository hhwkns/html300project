<template>
  <div id="app">
    <ul>
      <li v-for="link in
      links"> {{link}}</li>
    </ul>
    <div class=background><h1>Our Story</h1></div>
    <p>Our story begins in Oaxaca, Mexico in 1998, when Chef
      Ronaldo discovered his love of food.</p>
    <div class="chef">
      <div class="text">
        <h3>Chef Ronaldo</h3>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit,
          sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
          Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris
          nisi ut aliquip ex ea commodo consequat.Lorem ipsum dolor sit amet, consectetur adipiscing elit,
          sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
          Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris
          nisi ut aliquip ex ea commodo consequat</p>
          <button v-on:click="show = !show" class="btn">Contact Us</button>
          <h4 v-if="show">Thanks for connecting with us! Chef Ronaldo will respond to your message personally in 1-3 business days.</h4>


      </div>
      <div class="image">
        <img src="./assets/yucel-moran.jpg" alt="Chef Ronaldo" class="img">
      </div>
    </div>
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
show: true,
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

h4 {
  font-style: italic;
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
}

.btn {
  padding: .5rem;
  margin: .5rem;
  border-radius: 2px;
  background-color: gray;
  color: white;
  font-style: bold;
}

.chef {
  display: flex;
}

.img {
  width: 350px;
  height: 350px;
  object-fit: cover;
  flex-direction: column;
  margin: 1rem;
}

.text {
  text-align: justify;
  text-justify: inter-word;
  margin: 1rem;
}

</style>
