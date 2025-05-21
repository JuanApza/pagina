<template>
  <div class="grid grid-cols-1 md:grid-cols-3 gap-4 p-6">
    <PieChart :chartData="data1" :chartOptions="options1" />
    <PieChart :chartData="data2" :chartOptions="options2" />
    <PieChart :chartData="data3" :chartOptions="options3" />
  </div>
</template>

<script setup>
import PieChart from './PieChart.vue'

const data1 = {
  labels: ['Rojo', 'Azul', 'Amarillo'],
  datasets: [{
    label: 'Colores preferidos',
    data: [40, 30, 30],
    backgroundColor: ['#f87171', '#60a5fa', '#facc15']
  }]
}

const data2 = {
  labels: ['Chrome', 'Firefox', 'Safari'],
  datasets: [{
    label: 'Navegadores',
    data: [55, 25, 20],
    backgroundColor: ['#6366f1', '#10b981', '#fbbf24']
  }]
}

const data3 = {
  labels: ['Desktop', 'Tablet', 'Mobile'],
  datasets: [{
    label: 'Dispositivos',
    data: [50, 20, 30],
    backgroundColor: ['#34d399', '#f472b6', '#60a5fa']
  }]
}

const options1 = { responsive: true, plugins: { legend: { position: 'bottom' } } }
const options2 = { responsive: true, plugins: { legend: { position: 'bottom' } } }
const options3 = { responsive: true, plugins: { legend: { position: 'bottom' } } }
</script>