<script lang="ts">
	export let companyName: string;
    import FooterLink from "./FooterLink.svelte";
</script>

<footer>
	<section class="footer-copyright">
		<a href="/" >
			<img
				src="/assets/images/logo-ilojo-bar.webp"
				alt="Logo Ilojo Bar"
				width="200"
				height="auto"
				loading="lazy"
			/>
		</a>
		<p>&#169; {new Date().getFullYear()} {companyName}</p>
	</section>
	
	<section class="footer-links">
		<h2 class="footer-links__header">Menu</h2>
		<FooterLink link="/" linkTitle="Home" />
		<FooterLink link="/" linkTitle="Discover stories" />
	</section>

	<section class="footer-links">
		<FooterLink link="/spanish-migrant" linkTitle="Spanish migrant" />
		<FooterLink link="/the-returnees" linkTitle="The returnees" />
		<FooterLink link="/a-vip" linkTitle="A VIP" />
	</section>

	<section class="footer-links">
		<FooterLink link="/the-malaucay-connection" linkTitle="The Macaulay connection" />
		<FooterLink link="/a-family-house" linkTitle="A family house" />
		<FooterLink link="/slave-trade" linkTitle="Slave trade" />
	</section>

	<section class="footer-links">
		<FooterLink link="/botched-dreams" linkTitle="Botched dreams" />
		<FooterLink link="/a-angels-story" linkTitle="The Angel's Story" />
		<FooterLink link="/illegal-demolition" linkTitle="llegal demolition" />
	</section>
</footer>

<style>
	@font-face {
    font-family: 'Austral-Sans_Stamp-Regular';
    font-display: swap;
    src: url('/assets/fonts/AustralSansStamp-Regular.woff2') format('woff2'),
        url('/assets/fonts/AustralSansStamp-Regular.woff') format('woff');
    font-weight: normal;
    font-style: normal;
    font-display: swap;
}

@font-face {
    font-family: 'Black-Ground';
    font-display: swap;
    src: url('/assets/fonts/Black-Ground.woff') format('woff');
    font-weight: normal;
    font-style: normal;
}

	:global(body) {
    padding: 0;
    margin: 0;
		font-family: 'Austral-Sans_Stamp-Regular';
	}

	h2,
	p {
			padding: 0;
			margin: 0;
	}

	footer {
		padding: 3em;
		color: #fff;
		display: flex;
		justify-content: center;
		gap: 2em;
		background-color: #8c0500;
	}

	.footer-copyright {
		margin-right: 1em;
		text-align: center;
		display: flex;
		flex-direction: column;
		gap: .5em;
	}

	.footer-links {
		display: flex;
		flex-direction: column;
	}

	.footer-links__header {
		margin-bottom: .25em;
	}
</style>