<template>
  <div class="hello">
      <form action="" method="POST" name="formC">
    <p>
      <input type="text" v-model="utilisateur" placeholder="Nom utilisateur" required/>
      <input type="text" v-model="mdp" placeholder="Mot de passe" required/>
    </p>
    <p>
      <button type='button' v-on:click="test">About</button>
    </p>
      </form>
  </div>
</template>

<script>

export default {
  name: 'FormulaireConnexion',
  data: function() {
    return {
        utilisateur: "",
        mdp: ""
    }
  },
  methods: {
    test() {
        if(this.utilisateur === "admin" && this.mdp === "yannou"){
            alert("Tu est connecter !")
            this.utilisateur = ""
            this.mdp = ""
        }else{
            alert("Nom d'utilisateur ou/et mot de passe incorrecte !")
        }
    }
  }
}
</script>

<style type='text/scss' scoped>

</style>