<template>
	<div class="details">
		<div class="container">
			<div class="row">
				<div class="col-md-4">
					<img :src="products.image" class="img-fluid">
					<h3>{{products.productTitle}}</h3>
				</div>
			</div>
		</div>
	</div>
</template>
<script>
export default{
	name:'details',
	data(){
		return{
			title:"details",
			products: []
		}
	},
	created() {
		this.products = this.$route.params.mesaage;
	}

}
</script>
