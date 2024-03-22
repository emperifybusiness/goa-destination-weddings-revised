<script>
	import logo from '../lib/logo/asda.png';
	import video from '../lib/video/Timeline1.mov';
	import Slider from './Slider.svelte';
	import Story from './Story.svelte';
	import Services from './services.svelte';
</script>

<header>
	<div class="wrapper row">
		<button class="nav-toggle">
			<span class="icon-area"></span>
		</button>
		<a class="logo circle" href="/"><img height="60px" src={logo} alt="" srcset="" /></a>
		<nav class="nav">
			<ul>
				<li><a href="#">Home</a></li>
				<li><a href="#">About</a></li>
				<li><a href="#">Services</a></li>
				<li><a href="#">Portfolio</a></li>
				<li><a href="#">Contact</a></li>
			</ul>
		</nav>
	</div>
</header>

<div class="banner">
	<video autoplay muted loop id="myVideo">
		<source src={video} type="video/mp4" />
	</video>
	<div class="content">
		<h2>Love Blooms in Goa</h2>
		<p>And we are here to make it happen</p>
		<a href="/">Get Quote</a>
	</div>
</div>
<Story />
<Slider />

<style>
	.content p {
		font-family: 'Sail', system-ui;
		font-weight: 400;
		font-style: normal;
		font-size: 30px;
	}
	.circle {
		border-radius: 50%;
		height: 80px;
		border: #41005f 2px solid; 
		background: #ffffffa3;
		width: 90px;
		display: flex;
		justify-content: center;
		align-items: center;
	}
	.wrapper.s-y_bCXRrkrYfP.s-y_bCXRrkrYfP {
		width: 80%;
		display: flex !important;
		max-width: 1100px px;
		margin: 0 auto;
		position: relative;
	}
	.wrapper.s-y_bCXRrkrYfP.s-y_bCXRrkrYfP {
		width: 80%;
		max-width: 1100px;
		margin: 0 auto;
		position: relative;
		display: flex;
	}
	*,
	*::before,
	*::after {
		box-sizing: border-box;
	}
	body {
		margin: 0px !important;
		padding: 0px !important;
		font-family: 'Roboto', sans-serif;
		font-size: 1.3rem;
	}
	.wrapper {
		width: 80%;
		max-width: 1100px;
		margin: 0 auto;
		position: relative;
	}
	header {
		background: transparent;
		padding: 1em 0;
		text-align: center;
		position: absolute;
		width: 100%;
	}
	.nav {
		width: 100%;
	}
	.nav-toggle {
		cursor: pointer;
		border: 0;
		width: 3rem;
		height: 3rem;
		padding: 0em;
		background: transparent;
		color: rgb(255, 255, 255);
		transition: opacity 250ms ease;
		position: absolute;
		right: 0;
	}
	.nav-toggle:focus,
	.nav-toggle:hover {
		opacity: 0.75;
	}
	.icon-area {
		width: 50%;
		position: relative;
	}
	.icon-area,
	.icon-area::before,
	.icon-area::after {
		display: block;
		margin: 0 auto;
		height: 3px;
		background: white;
	}
	.icon-area::before,
	.icon-area::after {
		content: '';
		width: 100%;
	}
	.icon-area::before {
		transform: translateY(-6px);
	}
	.icon-area::after {
		transform: translateY(3px);
	}
	.nav {
		visibility: hidden;
		height: 0;
		position: absolute;
	}
	.nav ul {
		margin: 0;
		padding: 0;
		list-style: none;
	}
	.nav ul li a {
		color: #fff;
		text-decoration: none;
	}
	.openMenu {
		visibility: visible;
		height: auto;
		position: relative;
	}
	.logo {
		text-decoration: none;
		color: #fff;
		font-family: bebas neue;
		text-transform: uppercase;
		font-size: 40px;
	}
	@media (min-width: 800px) {
		.nav-toggle {
			display: none;
		}
		.nav {
			visibility: visible;
			display: flex;
			align-items: center;
			justify-content: flex-end;
			height: auto;
			position: relative;
		}
		.nav ul {
			margin: 0;
			display: flex;
			justify-content: space-between;
		}
		.nav ul li {
			margin: 0 0 0 1.5rem;
		}
		.row {
			display: flex;
			justify-content: space-between;
			align-items: center;
		}
	}

	.banner {
		background: linear-gradient(135deg, blueviolet, transparent), url('../lib/video/Timeline1.mov');
		height: 100vh;
		background-size: cover;
		background-position: center center;
		display: grid;
		place-items: center;
		text-align: center;
	}
	.banner video {
		position: absolute;
		top: 0;
		right: 0;
		z-index: -1;
		height: 100vh;
		width: 100%;
		object-fit: cover;
		background-position: center center;
		display: grid;
		place-items: center;
		text-align: center;
	}
	.content {
		margin-top: 0;
	}
	.content h2 {
		font-family: 'Rochester', cursive;
		font-weight: 500;
		font-style: normal;
		margin: 0;

		font-size: 104px;
		color: #fff;
	}
	.banner p {
		margin: 0;
		color: #fff;
	}
	.banner a {
		text-decoration: none;
		background: #800465;
		color: #fff;
		border: 2px solid white;
		padding: 19px 40px;
		border-radius: 50px;
		display: inline-block;
		margin-top: 15px;
		transition: 1s cubic-bezier(0.175, 0.885, 0.32, 1.275);
	}
	.banner a:hover {
		text-decoration: none;
		background: #ffffff;
		color: #000000;
		border: 2px solid rgb(81, 0, 85);
		padding: 19px 40px;
		border-radius: 50px;
		display: inline-block;
		margin-top: 15px;
	}
	@media (max-width: 991px) {
		.nav.openMenu {
			padding: 30px 0;
			background: rgba(0, 0, 0, 0.8);
			margin-top: 20px;
		}
		.nav.openMenu a {
			line-height: 2.5;
		}
	}
	@media (max-width: 600px) {
		.openMenu {
			padding: 5px 0;
			background: rgba(0, 0, 0, 0.8);
		}
		.openMenu a {
			color: #fff;
			font-size: 16px;
		}
		.content h2 {
			font-size: 35px;
		}
		.banner {
			background-position: 80%;
		}
		.logo {
			font-size: 40px;
		}
		.nav ul li {
			margin: 5px 0;
		}
		.content h2 {
			font-size: 35px;
		}
	}
</style>
