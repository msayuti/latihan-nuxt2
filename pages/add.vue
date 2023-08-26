<template>
  <div>
    <h1>Tambah Produk Baru</h1>
    <form @submit.prevent="addProduct">
      <label>Nama:</label>
      <input v-model="newProduct.name" required>
      <label>Deskripsi:</label>
      <textarea v-model="newProduct.description"></textarea>
      <label>Harga:</label>
      <input v-model.number="newProduct.price" required>
      <button type="submit">Tambah</button>
    </form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      newProduct: {
        name: '',
        description: '',
        price: 0
      }
    };
  },
  methods: {
    async addProduct() {
      // Panggil API untuk menambah produk baru
      await createProduct(this.newProduct);
      this.$router.push({ name: 'products' });
    }
  }
};
</script>
