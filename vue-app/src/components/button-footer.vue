<template>
  <div>
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
  name: "HelloWorld",
  data() {
    return {
      datos: [
        {
          nombre: "imagen1.png",
          usuario: "juan123",
          fecha: "2025-05-07 12:00",
          colores: 15423,
        },
        {
          nombre: "foto2.jpg",
          usuario: "ana456",
          fecha: "2025-05-06 18:22",
          colores: 13201,
        },
      ],
    };
  },
};
</script>
