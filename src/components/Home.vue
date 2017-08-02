<template>
	<div>
		<div>HOME页面</div>
		<div class="aa"  @click="Jump(123)">
			点我可以带参跳转哦
		</div>
	</div>

</template>

<script type="text/ecmascript-6">
    export default {
        methods: {
            //路由跳轉
            Jump(e) {
                this.$router.push({path:'/jump',query:{id:123}});
            }
        }
    }
</script>

<style>
.aa{
	color:red;
	cursor: pointer;
}
</style>
