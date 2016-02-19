<template>
	<h1>circleLine</h1>
	<div class="spinner1">
		<spinner1></spinner1>
	</div>
	<h2>dot</h2>
	<div class="spinner2">
		<spinner2></spinner2>
	</div>
</template>

<script>
import spinner1 from './components/circleLine'
import spinner2 from './components/dot'

export default {
    components: {
        spinner1,
        spinner2
    }
}
</script>

<style>
* {
	margin: 0;
	padding: 0;
}
body {
    font-family: Helvetica, sans-serif;
    overflow-x: hidden;
}
h2 {
	position: absolute;
	top: 80px;
	display: block;
}
.spinner2 {
	position: absolute;
	top: 120px;
	width: 100%;
}
</style>
