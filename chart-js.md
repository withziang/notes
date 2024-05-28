# React-chartjs-2 
Best graph framework

- [chartjs-2](https://react-chartjs-2.js.org/)
- `import {Bar, Line} from 'react-chartjs-2';`
- 
  ```
  import {
      Chart,
      CategoryScale,
      LinearScale,
      LineElement,
      PointElement,
      Title,
      Tooltip,
      Legend,
      BarElement
    } from 'chart.js';
## Bar 
```
            <Bar data={data} options={options} />

```

## Line 
```
            <Line data={data} options={options}/>

```


## Register !!
`// Register necessary components
Chart.register(CategoryScale, LinearScale, LineElement, PointElement, Title, Tooltip, Legend, BarElement);`
Tree shaved framework


## data
```
const data = {
    labels: ['x1', 'x2', 'x3', 'x4', 'x5'],
    datasets: [
        {
            label: 'x',
            backgroundColor: 'rgba(75,192,192,1)',
            borderColor: 'rgb(255,255,255)',
            borderWidth: 0,
            data: [1, 22, 5, 22, 55],
        },
    ],
};
```
```
const data = {
    labels: ...,
    datasets: [
        {
            label: 'x',
            backgroundColor: 'rgb(255,255,255)',
            borderColor: 'rgb(255,255,255)',
            borderWidth: 2,
            data: [1, 22, 5, 22, 55],
            fill: false, // Ensure the area under the line is not filled
            tension: 0
        },
    ],
};
```

## Options
```
const options = {
    scales: {
        x: {
            type: 'category',
            offset: true,
            grid: {
                display: true,
                color: 'rgba(200, 200, 200, 0.2)', // Custom grid color for x-axis
            },
        },
        y: {
            beginAtZero: true,
            grid: {
                display: true,
                color: 'rgba(200, 200, 200, 0.2)', // Custom grid color for y-axis
            },
            ticks: {
                stepSize: 10,
            },
        },
    },
    plugins: {
        title: {
            display: true,
            text: 'Total Statistic',
        },
        legend: {
            display: true,
            position: 'top',
        },
    },
};
const options_for_line = {
    scales: {
        x: {
            type: 'category',
            offset: true,
            grid: {
                display: true,
                color: 'rgba(200, 200, 200, 0.2)', // Custom grid color for x-axis
            },
        },
        y: {
            beginAtZero: true,
            grid: {
                display: true,
                color: 'rgba(200, 200, 200, 0.2)', // Custom grid color for y-axis
            },
            ticks: {
                stepSize: 10,
            },
        },
    },
    plugins: {
        title: {
            display: true,
            text: 'for the past 8 month',
        },
        legend: {
            display: true,
            position: 'top',
        },
    },
};
```
