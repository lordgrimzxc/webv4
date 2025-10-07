<template>
  <div>
    <h1>Inventory</h1>
    <table border="1" cellpadding="20" cellspacing="20">
      <thead>
        <tr>
          <th>Item Name</th>
          <th>Category</th>
          
        </tr>
      </thead>
      <tbody>
        <tr v-for="(item, index) in inventory" :key="index">
          <td>{{ item.name }}</td>
          <td>{{ item.category }}</td>
          
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script setup>
const inventory = [
  { name: 'Apple', category: 'Fruit',},
  
];
</script>

<style scoped>
table {
  width: 100%;
  border-collapse: collapse;
}


td {
  padding: 8px;
}
</style>
