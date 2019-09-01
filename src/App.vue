<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/Recurso.png" class="imge">
    <Title />
    <Section :sectionContent = "sectionContent"/>
    <Links :vals= "linkss" />
    <Footer />
  </div>
</template>

<script>
import Title from './components/Title'
import 'semantic-ui-css/semantic.min.css';
import Section from './components/Section'
import Footer from './components/footer'
import Links from './components/links'
export default {
  name: 'app',
  data: ()=>{
    return{
      linkss : [
      {link: "https://drive.google.com/open?id=10b-7gfpazXnhQf_5NAH8kevu1hk32jj8", desc: "Anexo 4"},
      {link: "https://drive.google.com/open?id=10b1qtgHCtgf1BLLsn9BFjUsIaM_YH0kS" , desc: "Anexo 3"},
      {link: "https://drive.google.com/open?id=10JPRSkUJYCHJ1X9_FNMeoTVDQKuU0ipv", desc: "Anexo 5"},
      {link: "https://drive.google.com/open?id=1nSQHSty84YK1VRp6Qayl80mzP8LmlqzI", desc: "Anexo 1"}
    ],
     sectionContent : [
       {imgDir : "1.jpeg"},
       {imgDir : "2.jpeg"},
       {imgDir : "3.jpeg"},
       {imgDir : "4.jpeg"},
       {imgDir : "5.jpeg"},
       {imgDir : "6.jpeg"},
       {imgDir : "7.jpeg"},
       {imgDir : "8.jpeg"},
       {imgDir : "9.jpeg"},
       {imgDir : "10.jpeg"}
     ]
    }
  },
  components: {
    Title,
    Section,
    Footer,
    Links 
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.imge {
  width: 300px;
  height: 300px;
}
</style>
