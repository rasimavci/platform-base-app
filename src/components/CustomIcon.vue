<template lang='pug'>
.custom-icon(@click='iconClicked')
  .icon-container
    i.icon.material-icons {{icon}}
  //- .name Application {{name.replace('icon','')}}
  .name {{name}}  
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
   //   window.open('https://platform2-29ov.onrender.com/', '_blank');
   if(this.name == "Sentiment Analizi")
      window.open('https://platform2-29ov.onrender.com/sentiment-analizi.html', '_blank');
   if(this.name == "Görüntü Analizi")
      window.open('https://platform2-29ov.onrender.com/goruntu-analizi.html', '_blank');      
    else if(this.name == "Müşteri Analitiği")
      window.open('https://platform2-29ov.onrender.com/musteri-analitigi.html', '_blank');
     else if(this.name == "Öneri Sistemleri")
      window.open('https://platform2-29ov.onrender.com/oneri-sistemleri.html', '_blank'); 
     else if(this.name == "Sosyal Medya Analizi")
      window.open('https://platform2-29ov.onrender.com/sosyal-medya-analizi.html', '_blank');       
    //  window.location.href = "https://platform2-29ov.onrender.com/";
   //   alert("Application " + this.name + " is not ready yet !")
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
