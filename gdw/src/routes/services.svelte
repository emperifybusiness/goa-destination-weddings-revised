<script>
	import video from '../lib/video/flowerpot.gif';
</script>

<section class="services sail-regular">
	<h1>The Beginning of Forever</h1>
	<img  src={video} alt="" srcset="" />

    <div class="story-container">

    </div>
</section>

<style>
.story-container{
    height: 10px;
    background-color: aqua;
}
.services{
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
}
    /* END story */
	.services img {
		height: 200px;
		width: auto;
	}
	#myVideo {
		height: 11px;
		width: 200px;
		border: 0px solid white;
	}
	.flowerContainer {
		width: 100%;
		height: auto;
	}
	.services {
		color: white;
		width: 100%;
		height: auto;
		text-align: center;
	}
	.services h1 {
		font-size: 60px;
		font-family: 'Sail', system-ui;
		font-weight: 500;
		margin-bottom: 0px;
		font-style: normal;
		color: rgba(172, 49, 172, 0.97);
	}
	.sail-regular {
		font-family: 'Sail', system-ui;
		font-weight: 400;
		font-style: normal;
	}
</style>
