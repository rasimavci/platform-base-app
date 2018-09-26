<template lang='pug'>
.custom-icon(@click='iconClicked')
  .icon-container
    i.icon.material-icons {{icon}}
  .name deneme {{name}}
</template>

<script>
export default {
  name: 'CustomIcon',
  data () {
    return {

    }
  },
  props: {
    icon: {
      type: String,
      required: true
    },
    name: {
      type: String,
      required: true
    }
  },
  methods: {
    iconClicked () {
      alert("You clicked icon: " + this.name)
    }
  }
}
</script>

<style scoped>
.custom-icon
.icon-container {
  display: inline-block;
  width: 90px;
  height: 90px;
  line-height: 90px;
  background-image: linear-gradient(141deg, #9fb8ad 0%, #1fc8db 51%, #2cb5e8 75%);
  border-radius: 20px;
  box-shadow: 10px 10px 5px #aaaaaa;
}
.icon{
  font-size: 35px;
}
.name {
  margin-top: 15px;
}
</style>
