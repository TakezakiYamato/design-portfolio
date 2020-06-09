<template>
  <div id="skill">
    <div class="skill-contents">
      <div class="skill-text">
        <h2>Skill</h2>
        <p>伝えたいユーザーに最適な体験を設計するためには、ものづくりに必要な工程を理解する必要があります。ビジネス、エンジニアリングと良質なコミュニケーションを取り、より良いプロダクトを生み出すためにデザインツールからフロントエンド言語まで扱えるようにしています。</p>
      </div>
      <div class="skill-category">
        <v-tabs
          v-model="model"
          centered
          color="#1D2B95"
        >
          <v-tab href="#tab-1">Design Software</v-tab>
          <v-tab href="#tab-2">Front End</v-tab>
          <v-tab href="#tab-3">Development Option</v-tab>
        </v-tabs>
        <v-tabs-items
          v-model="model"
        >
          <v-tab-item
            value="tab-1" 
          > 
            <div class="skill-content">
              <div class="skill-chip">
                <v-chip
                  class="chip"
                  v-for="design in designs" :key="design"
                  color="rgba(32, 42, 147, 0.88)"
                  text-color="white"
                >
                  {{ design }}
                </v-chip>
              </div>
              <div class="chart">
                <Design/>
              </div>
            </div>
          </v-tab-item>
          <v-tab-item
            value="tab-2"
          >
            <div class="skill-content">
              <div class="skill-chip">
               <v-chip
                  class="chip"
                  v-for="frontend in frontends" :key="frontend"
                  color="rgba(32, 42, 147, 0.88)"
                  text-color="white"
                >
                  {{ frontend }}
                </v-chip>
              </div>
              <div class="chart">
                <Front/>
              </div>
            </div>
          </v-tab-item>
          <v-tab-item
            value="tab-3"
          >
            <div class="skill-content">
              <div class="skill-chip">
                <v-chip
                  class="chip"
                  v-for="dev in devs" :key="dev"
                  color="rgba(32, 42, 147, 0.88)"
                  text-color="white"
                >
                  {{ dev }}
                </v-chip>
              </div>
              <div class="chart">
                <Devop/>
              </div>
            </div>
          </v-tab-item>
        </v-tabs-items>
      </div>
    </div>
  </div>
</template>
<script>
import Design from './Design';
import Front from './Front';
import Devop from './Devop';

export default {
  components: {
    Design,
    Front,
    Devop
  },
  data () {
    return {
      model: 'tab-1',
      designs: [
        'Adobe XD', 'Figma', 'Illustrator', 'Photoshop'
      ],
      frontends: [
        'HTML', 'CSS', 'Javascript', 'Vue'
      ],
      devs: ['Linux', 'Git', 'GitHub', 'Firebase'
      ]
    }
  }
}
</script>
<style scoped>
#skill {
  display: flex;
  justify-content: center;
}
.skill-contents {
  width:80%;
  height: auto;
  margin: 32px 0px;

}
.skill-text {
  margin-bottom: 32px;
}
.skill-text h2 {
  letter-spacing: 0.03em;
  padding-bottom: 10px;
}
.skill-text p {
  width: 62%;
  font-family: 'Noto Sans JP', sans-serif;
  font-size: 15px;
  letter-spacing: 0.05em;
  line-height: 1.7;
}
.skill-category {
  margin-top: 64px;
}
.skill-content {
  margin: 60px 4px;
  display: flex;
  justify-content: center;
  align-items: flex-start;
}
.skill-chip {
  margin-right: 32px; 
}
.chip {
  margin: 6px;
}
.chart {
  width: 60%;
  height: auto;
}
</style>
