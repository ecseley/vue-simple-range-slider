<template>
	
</template>

<script lang="ts">
import {Prop, Component, Vue} from 'vue-property-decorator';
import VueSimpleRangeSlider from './components/VueSimpleRangeSlider.vue';

@Component({
	components: {
		VueSimpleRangeSlider,
	},
})
export default class App extends Vue {
	value1 = [0, 10];
	value2 = 3;

	@Prop({default: 0}) activeWidth?: number;
}
</script>

<style lang="scss">
#app {
	font-family: Avenir, Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	text-align: center;
	color: #2c3e50;
	margin-top: 60px;
}
</style>
<style>
input {
	font-size: 30px;
}
</style>
