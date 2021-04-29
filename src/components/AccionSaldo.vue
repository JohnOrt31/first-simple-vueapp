<template>
  <button @click="accion" :disabled="desactivar" >{{ texto }} saldo</button>
</template>

<script>
export default {
    name: 'AccionSaldo',
    props: {
        texto: String,
        desactivar: {
            type: Boolean,
            default: false
        }
    }, 
    methods: {
        accion(){
            this.$emit('accion');
        }
    }

}
</script>

<style>

</style>