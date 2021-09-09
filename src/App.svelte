<script>
	export let name;
	import Summary from './Summary.svelte'
	import Projects from './Projects/Projects.svelte'
</script>

<main>
	<div id="pages">
		<div class="title-pic">
			<img class="ronald-img" alt="ronald" src="images/ronald.jpg">
			<div class="flex-vert">
				<h1>{name} Corona</h1>
				<h4>writes cool stuff</h4>
			</div>
		</div>
		<div id="main-content">
			<!-- <div id="main__grid"></div> -->
			<Summary/>
			
			<br><br>

			<Projects/>

			<br><br>

			<h3> Contact </h3>
			Ronaldmcorona@gmail.com
			<br> <a target="_blank" href="https://github.com/JomoPipi"
			>https://github.com/JomoPipi</a>
		</div>
	</div>
</main>

<style>

	#main-content {
		padding: 10%;
	}

	.ronald-img {
		width: 30%;
	}

	.title-pic {
		display: -webkit-box;
		display: -ms-flexbox;
		display: flex;
		-ms-flex-pack: distribute;
			justify-content: space-around;
		-webkit-box-align: center;
			-ms-flex-align: center;
				align-items: center;
		padding: 4%;
	}

/*# sourceMappingURL=styles.css.map */
</style>