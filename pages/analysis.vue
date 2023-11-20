
<template>
    <div class="md:min-h-[70vh]">
        <h1>Análisis</h1>
        <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-2 lg:grid-cols-2 gap-4">
            <p>{{ cseries }}</p>
            <p>{{ coptions }}</p>
            <apexchart :key="series" height="400" width="100%" type="line" :options="chartOptions" :series="series">
            </apexchart>
            <GraphTest />
            <GraphTest />
            <GraphTest />
            <GraphTest />
            <GraphTest />
        </div>
    </div>
</template>

<script setup>
import { ref } from 'vue'


const chartOptions = ref({
    chart: {
        id: "chart-energy-demand",
        type: "line",
    },
    dataLabels: {
        enabled: false
    },
    stroke: {
        curve: 'straight'
    },
    title: {
        text: 'Demanda de energía',
        align: 'left'
    },
    grid: {
        row: {
            colors: ['#f3f3f3', 'transparent'], // takes an array which will be repeated on columns
            opacity: 0.5
        },
    },
    xaxis: {
        categories: [1991, 1992, 1993, 1994, 1995, 1996, 1997, 1998],
    },
});
const series = ref([
    {
        name: "series-1",
        data: [30, 40, 35, 50, 49, 60, 70, 91],
    },
]);
</script>