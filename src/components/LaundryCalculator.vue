<template>
  <div class="laundry-calculator">
    <h1>Laundry Calculator</h1>
    <div class="input-group">
      <label for="pricePerKg">Harga per Kg (Rp):</label>
      <input type="number" id="pricePerKg" v-model="pricePerKg" min="0">
    </div>
    <div class="input-group">
      <label for="weight">Berat Pakaian (Kg):</label>
      <input type="number" id="weight" v-model="weight" min="0">
    </div>
    <div class="input-group">
      <label for="duration">Lama Pengerjaan (hari):</label>
      <input type="number" id="duration" v-model="duration" min="0">
    </div>
    <div class="input-group">
      <button @click="calculateTotal">Hitung Total</button>
    </div>
    <div v-if="total !== null" class="total">
      <h2>Total Harga: Rp {{ total }}</h2>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      pricePerKg: 0,
      weight: 0,
      duration: 0,
      total: null
    };
  },
  methods: {
    calculateTotal() {
      const totalPrice = this.pricePerKg * this.weight;
      const additionalCharge = this.duration * 5000; // Biaya tambahan per hari
      this.total = totalPrice + additionalCharge;
    }
  }
};
</script>

<style scoped>
.laundry-calculator {
  max-width: 400px;
  margin: auto;
  padding: 20px;
  border: 1px solid #ccc;
  border-radius: 5px;
}

.input-group {
  margin-bottom: 10px;
}

input[type="number"] {
  width: 100px;
  padding: 5px;
  border: 1px solid #0e0101;
  border-radius: 3px;
}

button {
  padding: 8px 15px;
  background-color: #150101;
  color: #fff;
  border: none;
  border-radius: 3px;
  cursor: pointer;
}

button:hover {
  background-color: #0056b3;
}

.total {
  margin-top: 20px;
}


</style>