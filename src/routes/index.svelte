<script>
	import Cta from '$lib/CTA.svelte';
	import Footer from '$lib/Footer.svelte';
	import Navbar from '$lib/Navbar.svelte';
	import Hero from '$lib/Hero.svelte';
	import Pricing from '$lib/Pricing.svelte';
	import Testimonials from '$lib/Testimonials.svelte';
	import WhyUs from '$lib/Why-us.svelte';
</script>

<Navbar/>
<Hero/>
<WhyUs/>
<Pricing/>
<div class="testimonials-wrapper"><Testimonials/></div>
<Cta/>
<Footer/>

<style>
.testimonials-wrapper{
	margin-left: 142px;
	margin-right: 104px;
	position: relative;
}

</style>