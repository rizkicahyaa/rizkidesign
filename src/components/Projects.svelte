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

	import GaviPoster from '../assets/poster-barca-gavi.png';
	import MessiPoster from '../assets/poster-messi.png';
	import BrunoPoster from '../assets/poster-mu-bruno.png';
	import GarnaPoster from '../assets/poster-mu-garnacho-remake.png';
	import PalmerPoster from '../assets/poster-chelsea-palmer.png';
	import MartinezPoster from '../assets/poster-inter-martinez.png';
</script>

<section class="projects py-5">
	<div class="container">
		<div class="row mb-4 border-bottom">
			<div class="col-md-2">
				<h1>PROJECTS</h1>
			</div>
		</div>
		<div class="row">
			<div class="col-md-4 g-2">
				<div class="card" data-aos="fade-up">
					<div class="card-body">
						<img src={GaviPoster} alt="" />
					</div>
				</div>
			</div>
			<div class="col-md-4 g-2">
				<div class="card">
					<div class="card-body">
						<img src={MessiPoster} alt="" />
					</div>
				</div>
			</div>
			<div class="col-md-4 g-2">
				<div class="card">
					<div class="card-body">
						<img src={BrunoPoster} alt="" />
					</div>
				</div>
			</div>
			<div class="col-md-4 g-2">
				<div class="card">
					<div class="card-body">
						<img src={GarnaPoster} alt="" />
					</div>
				</div>
			</div>
			<div class="col-md-4 g-2">
				<div class="card">
					<div class="card-body">
						<img src={PalmerPoster} alt="" />
					</div>
				</div>
			</div>
			<div class="col-md-4 g-2">
				<div class="card">
					<div class="card-body">
						<img src={MartinezPoster} alt="" />
					</div>
				</div>
			</div>
		</div>
	</div>
</section>
