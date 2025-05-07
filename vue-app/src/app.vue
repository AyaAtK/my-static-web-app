<template>
  <div id="app">
    <h1>Visor de Imágenes</h1>
    <table border="1">
      <thead>
        <tr>
          <th>Nombre</th>
          <th>Usuario</th>
          <th>Fecha</th>
          <th>Colores</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="(item, index) in datos" :key="index">
          <td>{{ item.nombre }}</td>
          <td>{{ item.usuario }}</td>
          <td>{{ item.fecha }}</td>
          <td>{{ item.colores }}</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      datos: [
        {
          nombre: 'imagen1.png',
          usuario: 'juan123',
          fecha: '2025-05-07 12:00',
          colores: 15423,
        },
        {
          nombre: 'foto2.jpg',
          usuario: 'ana456',
          fecha: '2025-05-06 18:22',
          colores: 13201,
        },
      ],
    };
  },
};
</script>

<style>
body {
  font-family: Arial, sans-serif;
  margin: 2rem;
}
table {
  border-collapse: collapse;
  width: 100%;
}
th,
td {
  padding: 8px;
  text-align: left;
}
th {
  background-color: #f2f2f2;
}
</style>
