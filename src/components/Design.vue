<script>
import { Radar } from 'vue-chartjs'

export default {
  extends: Radar,
  data () {
    return {
      data: {
        label: [],
        datasets: [{
          data: [],
          label: 'Design Software',
          backgroundColor: 'grey',
        }]
      }
    }
  },
  mounted () {
    this.renderChart(this.data, this.options)
  }
}
</script>

