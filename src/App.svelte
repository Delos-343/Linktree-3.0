<script>
	import Button from "./components/Button.svelte";
	import Socials from "./components/Socials.svelte";

	let links = [
		{title: "Instagram", url: "https://instagram.com/f_dwi.han"},
		{title: "Github", url: "https://github.com/Delos-343/"},
		{title: "LinkedIn", url: "https://www.linkedin.com/in/fachry-dwi-han/"},
		{title: "Codepen", url: "https://codepen.io/Delos_343/"},
		{title: "Portfolio", url: "https://fachry-dwihan.netlify.app/"},
	];

	let sosmed = [
		{icons: "©", url: "./assets/sig-2021.png"},
		{icons: "✉", url: "mailto:mohammed.dwihandoko@gmail.com"},
		{icons: "✆", url: "tel:+6287788763027"},
	];
</script>

<div class="container-center">
	<img
		src="https://i.postimg.cc/vHbd3YbC/my-signature-2021-no-bg.png"
		alt="signature"
		class="profile-picture"
	/>

	<p class="username"> @f.dwi_han </p>

	{#each links as link}
		<Button {...link} />
	{/each}
</div>
<div class="container-center">

	<p class="username"> Contact Me </p>

	{#each sosmed as socials}
		<Socials {...socials} />
	{/each}
</div>

<style>

	img.profile-picture {
		width: 120px;
		margin-top: 35px;
		border-radius: 50%;
		object-fit: cover;
		border: 2px solid #c0c0c0;
		background-color: #fff;
	}

	p.username {
		margin-bottom: 50px;
		font-weight: 600;
		font-size: 1.5rem;
	}

	.container-center {
		text-align: center;
		padding: 5%;
		background-color: #242526;
		color: #fff;
	}

</style>
