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
          <v-tab href="#tab-2">Programming Language</v-tab>
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
                  v-for="skill in skills" :key="skill.design"
                  color="rgba(32, 42, 147, 0.88)"
                  text-color="white"
                >
                  {{ skill.design }}
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
            <div class="skill-tip">
              <v-chip>HTML</v-chip>
            </div>
          </v-tab-item>
          <v-tab-item
            value="tab-3"
          >
            <div class="skill-tip">
              <v-chip>Git</v-chip>
            </div>
          </v-tab-item>
        </v-tabs-items>
      </div>
    </div>
  </div>
</template>
<script>
import Design from './Design';

export default {
  components: {
    Design
  },
  data () {
    return {
      model: 'tab-1',
      skills: [
        { design: 'Adobe XD' },
        { design: 'Figma' },
        { design: 'Illustrator' },
        { design: 'Photoshop' }
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
.skill-text p {
  width: 62%;
  font-family: 'Noto Sans JP', sans-serif;
  font-size: 15px;
}
.skill-content {
  margin: 48px 4px;
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
