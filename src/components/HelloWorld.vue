<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
      En 2021, j'était en 2ème année de BTS SIO option SLAM.
    </p>
    <p>
      <button type='button' v-on:click="$router.push({ path: 'about' })" class='home-b'>About</button><br>
      <button type='button' v-on:click="$router.push({ path: 'connexion' })" class='home-b'>Connexion</button>
    </p>
    <h2>Réseau sociaux</h2>
    <ul>
      <li><a href="https://fr-fr.facebook.com/yann.hittin" target="_blank" rel="noopener">Facebook</a></li>
      <li><a href="https://www.instagram.com/yannhittin/" target="_blank" rel="noopener">Instagram</a></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<style type='text/scss' scoped>
h2 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;   
}

a {
  color: #42b983;
}

.home-b {
  border: 0;
    line-height: 2.5;
    padding: 0 20px;
    font-size: 1rem;
    text-align: center;
    color: black;
    border-radius: 10px;
    background-color: #33CEFF;
    background-image: linear-gradient(to top left,
                                      rgba(0, 0, 0, .2),
                                      rgba(0, 0, 0, .2) 30%,
                                      rgba(0, 0, 0, 0));
    box-shadow: inset 2px 2px 3px rgba(255, 255, 255, .6),
                inset -2px -2px 3px rgba(0, 0, 0, .6);
}

</style>
