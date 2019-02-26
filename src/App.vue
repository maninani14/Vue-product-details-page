<template>
	<div id="app">
		<div class="nav-bar">
			<ul>
				<li>
					<router-link to="/">Products Details Page</router-link>
				</li>
			</ul>
		</div>
		<router-view/>
	</div>
</template>

<style>
#app {
	font-family: "Work Sans", sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	text-align: center;
	color: #2c3e50;
	-webkit-font-smoothing: antialiased;
}
.nav-bar{
	background: #123;
	padding: 25px 0;
}
.nav-bar a{
	margin-right: 40px;
	font-size: 1.5em;
	color: #fff;
}
</style>
