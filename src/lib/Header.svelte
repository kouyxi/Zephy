<script>
	import Logo from './assets/Logo.svelte';
</script>

<header>
	<div class="container header__container">
		<nav>
			<a href="/" class="logo"><Logo /> <span class="logo-text">Zephy</span></a>
			<ul>
				<li><a href="/projects">Projects</a></li>
				<li><a href="/about">About us</a></li>
				<li><a href="/team">Our Team</a></li>
				<li><a href="/services">Services</a></li>
			</ul>
			<a href="/" class="btn">Get a Quote!</a>
		</nav>
	</div>
</header>

<style>
	nav {
		padding-top: 16px;
		padding-bottom: 16px;
		display: flex;
		font-family: var(--heading-font);
		align-items: center;
	}
	nav ul {
		display: flex;
		gap: 30px;
		margin-left: auto;
		margin-right: auto;
	}
	ul a {
		position: relative;
	}
	ul a::before {
		content: '';
		width: 0%;
		height: 1px;
		position: absolute;
		top: 22px;
		background-color: black;
	}
	ul a:hover::before {
		width: 100%;
		transition: 200ms;
	}
	.logo {
		display: flex;
		gap: 5px;
		align-items: center;
	}
	.logo-text {
		font-size: 1.5rem;
		font-weight: 600;
		font-family: var(--body-font);
	}
</style>
