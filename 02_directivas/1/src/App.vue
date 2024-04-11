<script setup>
const datos = ref({
    nombre: '',
    apellido: ''
});
</script>

<template>
    <div class="container pt-5">
        <h1>Datos Personales</h1>
        <div class="card col-4 p-3">
            <div class="mb-3">
                <label class="form-label" for="nombre">Nombre</label>
                <input class="form-control" id="nombre" type="text" v-model="datos.nombre"/>
            </div>
            <div class="mb-3">
                <label class="form-label" for="apellido">Apellido</label>
                <input class="form-control" id="apellido" type="text" v-model="datos.apellido"/>
            </div>
            <div class="card-text ">
                <p>Tu nombre completo es: {{datos.nombre}} {{datos.apellido}}</p>
            </div>
        </div>
    </div>
</template>

<style scoped>
</style>
