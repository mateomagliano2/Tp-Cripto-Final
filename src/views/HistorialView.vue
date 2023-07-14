<template>
  <div>
    <h2>Historial de transacciones</h2>
    <table>
      <thead>
        <tr>
          <th>Criptomoneda</th>
          <th>Cantidad</th>
          <th>Fecha y hora</th>
          <th>Precio</th>
          <th>Acciones</th>
        </tr>
      </thead>
      <!-- <tbody>
         <tr v-for="transaction in transactions" :key="transaction._id">
          <td>{{ transaction.cryptocurrency }}</td>
          <td>{{ transaction.amount }}</td>
          <td>{{ transaction.date }}</td>
          <td>{{ transaction.price }}</td>
          <td> -->
            <!-- <button @click="editTransaction(transaction)">Editar</button>
            <button @click="deleteTransaction(transaction)">Borrar</button>
          </td>
        </tr>
      </tbody> -->
    </table>
  </div>
</template>

<script>
//export default {
//  data() {
//    return {
//      transactions: []
//    }
//  },
//  created() {
//    fetch(`https://laboratorio3-f36a.restdb.io/rest/transactions?q={"user_id": "${this.$store.state.userId}"}`, {
//      headers: {
//        'Content-Type': 'application/json',
//        'x-apikey': 'TU_API_KEY' // Reemplazar con tu API Key
//      }
//    })
//      .then(response => response.json())
//      .then(data => {
//        this.transactions = data
//      })
//  },
//  methods: {
//    editTransaction(transaction) {
//      Implementar la lógica para editar una transacción
//    },
//    deleteTransaction(transaction) {
//      Implementar la lógica para borrar una transacción
//    }
//  }
//}
</script>