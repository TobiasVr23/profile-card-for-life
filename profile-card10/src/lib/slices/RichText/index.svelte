<script>
	import { PrismicRichText } from '@prismicio/svelte';
	import { PrismicImage } from '@prismicio/svelte';
	import Label from './Label.svelte';

	/** @type {import("@prismicio/client").Content.RichTextSlice} */
	export let slice;
</script>
<body>
	<div class="card">
		<div class="avatar">
			<PrismicImage field={slice.primary.avatar} />
		</div>

		<div class="name">
			<h1>Tobias Vrolijk</h1>
		</div>

		<div class="github-link">
		   <a href="https://github.com/TobiasVr23" target="_blank">
			<PrismicImage field={slice.primary.githubimage} />
		   </a>
		</div>

		<div class="description1">
			<PrismicImage field={slice.primary.locationname} /><h2>Amsterdam</h2>
		</div>
		<div class="description2">
			<h2>📅 31-03-2003</h2>
		</div>

	</div>
</body>

<style>
	.card{
		height: 100vh;
		width: 25em;
		background: rgb(85,139,245);
		background: linear-gradient(180deg, rgba(85,139,245,1) 60%, #ffd09c 100%);
		border-radius: 15px;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.description1{
		display: flex;
		flex-direction: row;
		align-items: center;
		justify-content: space-evenly;
	}




</style>
