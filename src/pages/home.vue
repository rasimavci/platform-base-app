<template lang='pug'>
f7-page(lang="pug")
  .navbar
    .navbar-inner
      .left
        a.link.icon-only.panel-open(href="#" data-panel="left")
          i.icon.f7-icons.ios-only menu
          i.icon.material-icons.md-only menu
      .title.sliding Eğitim Platformu
      .right
        a.link.icon-only.panel-open(href="#" data-panel="right")
          i.icon.f7-icons.ios-only menu
          i.icon.material-icons.md-only menu
  f7-block(strong="")
    .row.no-gap
      .col-50.tablet-25.desktop-25.margins(v-for='i in mockData')
        custom-icon(:icon='i.icon', :name='i.name')

</template>
<script>
import CustomIcon from '../components/CustomIcon'

let mockIcons = [
  '3d_rotation',
  'alarm',
  'aspect_ratio',
  'build',
  'account_circle',
  'fingerprint',
  'hourglass_empty',
  'donut_small',
  'g_translate',
  'grade'
]
export default {
  name: 'home',
  data () {
    return {
      mockData: [
        // {
        //   id: 1,
        //   name: 'icon 1',
        //   icon: '3d_rotation'
        // }
      ]
    }
  },
  components: {
    customIcon: CustomIcon
  },
  mounted () {
    this.generateMockData ()
  },
  methods: {
    generateMockData () {
      for(let i = 0; i< 12; i++) {
        this.mockData.push({
          id: i,
          name: 'icon ' + i,
          icon: mockIcons[Math.floor(Math.random()*10)]
        })
      }
      debugger
    }
  }
}
</script>
<style scoped>
.margins {
  margin: 5px 0 5px 0;
  text-align: center;
}
</style>

