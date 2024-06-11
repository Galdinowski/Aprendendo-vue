<template>
    <div>
      <table border="1">
        <thead>
          <tr>
            <th>Month</th>
            <th>Simple Interest</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="month in months" :key="month">
            <td>{{ month }}</td>
            <td>{{ calculateInterest(month) }}</td>
          </tr>
        </tbody>
      </table>
    </div>
  </template>
  
  <script>
  export default {
    name: 'TableComponent',
    props: {
      principal: {
        type: Number,
        required: true
      },
      rate: {
        type: Number,
        required: true
      },
      months: {
        type: Number,
        required: true
      }
    },
    methods: {
      calculateInterest(month) {
        const annualRate = this.rate / 100;
        const timeInYears = month / 12;
        const interest = (this.principal * annualRate * timeInYears)+this.principal;
        return interest.toFixed(2);
      }
    }
  };
  </script>
  
  <style scoped>
  table {
    width: 100%;
    border-collapse: collapse;
  }
  
  th, td {
    padding: 8px;
    text-align: left;
  }
  </style>
  