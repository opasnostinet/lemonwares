<script>
	import Cta from "$lib/CTA.svelte";
	import Footer from "$lib/Footer.svelte";
	import Navbar from "$lib/Navbar.svelte";
	import Hero from "$lib/Hero.svelte";
	import Pricing from "$lib/Pricing.svelte";
	import Testimonials from "$lib/Testimonials.svelte";
	import Portfolio from "$lib/Portfolio.svelte";
	import WhyUs from "$lib/Why-us.svelte";
</script>

<Navbar />
<Hero />
<WhyUs />
<Pricing />
<div class="testimonials-wrapper"><Testimonials /></div>
<div class="portfolio-wrapper"><Portfolio /></div>
<div class="call-to-action-wrapper"><Cta /></div>
<Footer />

<style>
	.testimonials-wrapper {
		margin-left: 142px;
		margin-right: 104px;
		position: relative;
	}
	.portfolio-wrapper {
		margin: 84px 106px 110px 140px;
	}

	.call-to-action-wrapper {
		margin: 80px;
	}

	@media (max-width: 900px) {
		.testimonials-wrapper {
			margin-left: 11%;
			margin-right: 11%;
		}
	}

	@media (max-width: 650px) {
		.testimonials-wrapper {
			margin-left: 8%;
			margin-right: 8%;
		}
	}
	@media (max-width: 800px) {
		.portfolio-wrapper {
			margin: 3%;
		}
	}
	@media (max-width: 1100px) {
		.call-to-action-wrapper {
			margin: 3%;
		}
	}
</style>
