<script>
	import AOS from 'aos';
	import 'aos/dist/aos.css';
	import { onMount } from 'svelte';

	onMount(() => {
		AOS.init({
			duration: 1000,
			once: true
		});
	});

	const projects = [
		{
			name: 'Gavi Poster',
			image: '/images/poster-barca-gavi.png'
		},
		{
			name: 'Messi Poster',
			image: '/images/poster-messi.png'
		},
		{
			name: 'Bruno Poster',
			image: '/images/poster-mu-bruno.png'
		},
		{
			name: 'Garna Poster',
			image: '/images/poster-mu-garnacho-remake.png'
		},
		{
			name: 'Chelsea Poster',
			image: '/images/poster-chelsea-palmer.png'
		},
		{
			name: 'Martinez Poster',
			image: '/images/poster-inter-martinez.png'
		},
		{
			name: 'Jones Poster',
			image: '/images/poster-ipul-jones.png'
		}
	];
</script>

<section class="projects py-5">
	<div class="container">
		<div class="row mb-4 border-bottom">
			<div class="col-md-2">
				<h1>PROJECTS</h1>
			</div>
		</div>
		<div class="row">
			<h4>Poster</h4>
			{#each projects as project}
				<div class="col-md-4 g-2">
					<div class="card" data-aos="flip-left">
						<div class="card-body">
							<img src={project.image} alt="" />
						</div>
					</div>
				</div>
			{/each}
		</div>
	</div>
</section>
