 <template>
  <div>
    <Header/>
    <HelloWorld/>
    <LifeCycle/>
    <Pessoa/>
  </div>
 </template>

 <script>
 import Header from './components/09 - Header.vue'
 import HelloWorld from './components/01 - HelloWorld.vue'
 import LifeCycle from './components/02 - LifeCycle.vue'
 import Pessoa from './components/03 - Pessoa.vue'


 export default {
  name: 'App',
  components: {
    Header,
    HelloWorld,
    LifeCycle,
    Pessoa

  }
 }
</script>

<style>
  body{
    background: #333;
    color: #fff;
  }

  a {
    color: red;
  }

  .p-text {
    color: greenyellow;
  }

</style>