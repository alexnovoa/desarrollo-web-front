<template>
  <div>
    {{nombre}}
      <ul>
        <li v-for="item in clientes" :key="item.id">
            {{item.nombre}}
        </li>
      </ul>
  </div> 
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data () {
    return {
      nombre : 'Alex',
      mostrar : true,
      clientes : [{id:1, nombre : 'Alex'},{id:2, nombre : 'Luis'}]
    }
  },
  methods : {
    metodo1 () {
        console.log('Ingresa al metodo')
    }
  }
}
</script>

<style scoped>
li {
  color: blue;
  font-size: 34px;
}
</style>
