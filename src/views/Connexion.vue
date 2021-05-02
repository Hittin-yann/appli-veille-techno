<template>
<div>
    <div>
        <h1>Connexion</h1>
    </div>
    <div>
        <formulaire-connexion></formulaire-connexion>
    </div>
</div>
</template>

<script>
// @ is an alias to /src
import FormulaireConnexion from '@/components/FormulaireConnexion.vue'

export default {
  name: 'Connexion',
  components: {
    FormulaireConnexion 
  }
}
</script>

<style>

</style>