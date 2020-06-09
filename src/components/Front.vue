<script>
import { Radar } from 'vue-chartjs'

export default {
  extends: Radar,
  data () {
    return {
      data: {
        label: false,
        labels: ["HTML", "CSS", "Javascript", "Vue"],
        datasets: [{
          data: [4, 4, 3, 3],
          label: false,
          borderColor: 'rgba(32, 42, 147, 0.85)',
          borderWidth: 1,
          backgroundColor: 'rgba(32, 42, 147, 0.65)',
          pointRadius: 0,
          fontColor: 'white',
          fontSize: 16
        }]
      },
      options: {
        legend: {
          display: false
        },
        tooltips: {
          enabled: false
        },
        scale: {
          pointLabels: {
            fontSize: 14,
            fontColor: 'rgba(32, 42, 147, 0.95)',
            fontFamily: "'Montserrat', sans-serif"
          },
          ticks: {
            max: 5,
            stepSize: 1,
            beginAtZero: true
          }
        }
      }
    }
  },
  mounted () {
    this.renderChart(this.data, this.options)
  }
}
</script>

