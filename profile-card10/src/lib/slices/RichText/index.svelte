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
		<div class="description">
			<PrismicImage field={slice.primary.githubimage} />
			<PrismicImage field={slice.primary.locationname} />
		</div>
		

	</div>
</body>

<style>
	.card{
		height: 100vh;
		width: 25em;
		background: rgb(85,139,245);
		background: linear-gradient(180deg, rgba(85,139,245,1) 35%, rgba(204,221,255,1) 100%);
		border-radius: 15px;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}
	.name{
		margin-top: 3em;
	}

</style>
