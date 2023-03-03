<script lang="ts">
	export let src: string;
	export let alt: string;
	export let title: string;
	export let url: string;
</script>

<main>
	<div class="front">
		<img class="rounded" {src} {alt} />
	</div>
	<div class="back">
		<h1 class="texto-fluido">{title}</h1>
		<p><a href={url}>Mas detalles</a></p>
	</div>
</main>

<style>
	main {
		display: flex;
		justify-content: center;
		align-items: center;
	}
	a{
		color: white;
		transition: 0.2s ease-in-out;
	}
	a:hover{
		color: rgb(201, 197, 197);
	}
	img {
		width: 35rem;
		height: 25rem;
	}

	.front {
		transition: 200ms;
		backface-visibility: hidden;
	}
	.back {
		width: 35rem;
		height: 25rem;
		background-color: #2072AA;
		backface-visibility: hidden;
		position: absolute;
		transition: 200ms;
		transform: perspective(600px) rotateY(-180deg);
		display: flex;
		align-items: center;
		justify-content: center;
		flex-direction: column;
		border: 1px solid white;
		border-radius: 0.5rem;
	}

	.back h1,
	p {
		text-align: center;
		width: 25vw;
	}

	main:hover > .front {
		transform: perspective(600px) rotateY(-180deg);
	}

	main:hover > .back {
		transform: perspective(600px) rotateY(0deg);
	}

	.texto-fluido{
		background-image: linear-gradient(90deg,
		#ffaebc, #a0e7e5, #b4f8c8, #fbe7c6);
		background-size: 400%;
		color: transparent;
		font-weight: bold;
		background-clip: text;
		-webkit-background-clip: text;
		animation: text-gradient 4s infinite alternate;
	}

	@keyframes text-gradient {
		0%{
			background-position: left;
		}
		100%{
			background-position: right;
		}
	}
</style>
