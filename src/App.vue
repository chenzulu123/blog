<template>
  <div id="app">
    <my-header></my-header>
    <div class="main">
      <router-view></router-view>
    </div>
    <my-footer></my-footer>
  </div>
</template>

<script>
import MyHeader from './components/Header.vue';
import MyFooter from './components/Footer.vue';

export default {
	name: 'app',
	components: {
		MyHeader,
		MyFooter,
	},
};
</script>

<style lang="less">

html,
body {
	padding: 0;
	margin: 0;
	height: 100%;
	width: 100%;
}
#app {
	font-family: 'Avenir', Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  height: 100%;
  .main{
    height: calc(100% - 156px);
    overflow-y: auto;
    margin: 0;
    padding: 0;
  }
}
</style>
