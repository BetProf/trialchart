<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Interactive Chart</title>
  <style>
    body {
      font-family: sans-serif;
      padding: 24px;
      background: #fff;
      color: #111;
    }
    select {
      font-size: 13px;
      padding: 6px 10px;
      border: 0.5px solid #ccc;
      border-radius: 8px;
      background: #fff;
      cursor: pointer;
    }
  </style>
</head>
<body>

  <div style="display: flex; justify-content: space-between; align-items: center; margin-bottom: 16px; flex-wrap: wrap; gap: 8px;">
    <div>
      <p style="margin: 0; font-size: 13px; color: #666;">Total revenue</p>
      <p style="margin: 0; font-size: 24px; font-weight: 500;" id="total">$0</p>
    </div>
    <select id="chartType">
      <option value="bar">Bar chart</option>
      <option value="line">Line chart</option>
      <option value="doughnut">Doughnut chart</option>
    </select>
  </div>

  <div style="display: flex; flex-wrap: wrap; gap: 16px; margin-bottom: 12px; font-size: 12px; color: #666;">
    <span style="display: flex; align-items: center; gap: 4px;">
      <span style="width: 10px; height: 10px; border-radius: 2px; background: #534AB7; display:inline-block;"></span>
      Monthly sales
    </span>
  </div>

  <div style="position: relative; width: 100%; height: 300px;">
    <canvas id="myChart" role="img" aria-label="Monthly sales chart showing data from January to June">
      Jan 42k, Feb 58k, Mar 51k, Apr 76k, May 63k, Jun 89k.
    </canvas>
  </div>

  <script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/4.4.1/chart.umd.js"></script>
  <script>
    const labels = ['Jan','Feb','Mar','Apr','May','Jun'];
    const values = [42000, 58000, 51000, 76000, 63000, 89000];

    const total = values.reduce((a, b) => a + b, 0);
    document.getElementById('total').textContent = '$' + (total / 1000).toFixed(0) + 'k';

    const ctx = document.getElementById('myChart');

    let chartInstance = new Chart(ctx, {
      type: 'bar',
      data: {
        labels,
        datasets: [{
          label: 'Sales',
          data: values,
          backgroundColor: '#AFA9EC',
          borderColor: '#534AB7',
          borderWidth: 1.5,
          borderRadius: 4,
          pointBackgroundColor: '#534AB7',
          fill: true
        }]
      },
      options: {
        responsive: true,
        maintainAspectRatio: false,
        plugins: { legend: { display: false } },
        scales: {
          y: {
            ticks: { callback: v => '$' + (v/1000).toFixed(0) + 'k', font: { size: 11 } },
            grid: { color: 'rgba(128,128,128,0.1)' }
          },
          x: {
            ticks: { font: { size: 11 } },
            grid: { display: false }
          }
        }
      }
    });

    document.getElementById('chartType').addEventListener('change', function() {
      const type = this.value;
      chartInstance.destroy();
      chartInstance = new Chart(ctx, {
        type,
        data: {
          labels,
          datasets: [{
            label: 'Sales',
            data: values,
            backgroundColor: type === 'doughnut'
              ? ['#AFA9EC','#5DCAA5','#F0997B','#85B7EB','#FAC775','#ED93B1']
              : '#AFA9EC',
            borderColor: type === 'doughnut'
              ? ['#534AB7','#1D9E75','#D85A30','#378ADD','#BA7517','#D4537E']
              : '#534AB7',
            borderWidth: 1.5,
            borderRadius: type === 'bar' ? 4 : 0,
            pointBackgroundColor: '#534AB7',
            fill: type === 'line'
          }]
        },
        options: {
          responsive: true,
          maintainAspectRatio: false,
          plugins: { legend: { display: false } },
          scales: type === 'doughnut' ? {} : {
            y: {
              ticks: { callback: v => '$' + (v/1000).toFixed(0) + 'k', font: { size: 11 } },
              grid: { color: 'rgba(128,128,128,0.1)' }
            },
            x: {
              ticks: { font: { size: 11 } },
              grid: { display: false }
            }
          }
        }
      });
    });
  </script>

</body>
</html>
