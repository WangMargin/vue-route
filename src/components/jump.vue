<template>
	<div>
		<div @click="param">下面是我带过来的参数哦！</div>
		<p>{{this.$route.query.id}}</p>
	</div>
	
</template>

<script>
	export default {
        methods: {
            //路由跳轉
            param() {
                console.log(this.$route.query.id);
            }
        }
    }
</script>

<style>
</style>