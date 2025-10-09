<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import CenteredTextOnlyHero from "$lib/components/layout/hero-sections/CenteredTextOnlyHero.svelte";
</script>

<CenteredTextOnlyHero
	title="Persistent ocean operations without limits"
	subtitle="Deploy autonomous surface and underwater vehicles that operate for months at a time, capturing critical data and executing missions at 10x lower cost than legacy systems."
	imageSrc="/generated/image-a-wide-atmospheric-photograph-of-a-diver.webp"
/>
<LogoScroller
	label="Trusted by leading defense, research, and conservation organizations"
	logoUrls={[
		'https://cdn.brandfetch.io/navy.mil/w/400/h/400/logo',
		'https://cdn.brandfetch.io/noaa.gov/w/400/h/400/logo',
		'https://cdn.brandfetch.io/nature.org/w/400/h/400/logo',
		'https://cdn.brandfetch.io/onr.navy.mil/w/400/h/400/logo'
	]}
/>

<Summary
	title="The Ulysses difference"
	text="Ulysses delivers the only integrated autonomous surface and underwater vehicle system that deploys, retrieves, and recharges subsea robots without human intervention. We serve defense commands, offshore operators, and conservation organizations who need persistent ocean operations spanning months rather than hours. By eliminating expensive support vessels and enabling real-time data at scale, we make critical subsea missions accessible at one-tenth the cost of legacy systems."
/>

<Testimonials
	testimonials={[
		{
			name: "Dr. Elena Vasquez",
			position: "Lead Marine Scientist",
			company: "The Nature Conservancy",
			quote:
				"Ulysses mapped 200 hectares of seagrass habitat in three days, a survey that would have taken our team six weeks by traditional methods. The autonomous system delivered higher-resolution data while freeing our scientists to focus on analysis and restoration planning.",
			image: "/generated/image-professional-headshot-of-a-confident-fem.webp"
		},
		{
			name: "Commander James Mitchell",
			position: "Program Manager, Mine Countermeasures",
			company: "Naval Sea Systems Command",
			quote:
				"The Mako system costs a fraction of our legacy AUVs and eliminates the need for dedicated support vessels. We can now maintain persistent subsea surveillance for months at operational tempos that were previously impossible within our budget constraints.",
			image: "/generated/image-professional-headshot-of-a-confident-mal.webp"
		},
		{
			name: "Marcus Chen",
			position: "Director of Subsea Operations",
			company: "Pacific Energy Infrastructure",
			quote:
				"The dual-domain capability changed our risk calculus entirely. We now conduct pipeline inspections in weather windows that would have grounded our traditional ROV operations. The 72-hour endurance means we complete surveys in a single deployment instead of multiple mobilizations.",
			image: "/generated/image-professional-headshot-of-a-confident-mal.webp"
		}
	]}
/>

<Features
	title="Capabilities that redefine ocean operations"
	subtitle="Industry-first technology that delivers persistent, autonomous missions at unprecedented scale and cost efficiency."
	features={[
		{
			title: "Dual-domain autonomy",
			description:
				"Our integrated ASV-AUV system autonomously deploys, retrieves, and recharges underwater vehicles through proprietary ALARS technology. No support vessels required for multi-month operations."
		},
		{
			title: "Persistent operations",
			description:
				"Execute missions continuously for months at a time with automated launch and recovery cycles. Each Mako delivers up to 72-hour endurance per charge across 150 nautical miles."
		},
		{
			title: "10x cost advantage",
			description:
				"Deploy swarms of $25,000 attritable Mako AUVs instead of single legacy systems. Achieve mission objectives at dramatically lower capital and operational costs."
		},
		{
			title: "Real-time intelligence",
			description:
				"Stream sensor data and maintain control during subsea operations through continuous surface-to-subsea connectivity. Make mission-critical decisions with live intelligence."
		},
		{
			title: "Extreme adaptability",
			description:
				"Rapidly reconfigure for defense, commercial, or restoration missions using modular payloads and universal interconnectors. One platform, unlimited applications across the $600B ocean services market."
		},
		{
			title: "Precision at depth",
			description:
				"Operate to 1,000 feet with advanced navigation combining DVL, IMU, and full-INS compatibility. Equipped with side-scan sonar, multi-beam sonar, and AI-powered vision systems for mission success."
		}
	]}
/>
<AboutTeaser />
<CallToAction
	title="Ready to achieve persistent subsea operations?"
	subtitle="Schedule a technical briefing"
	description="Defense program managers at NAVSEA and ONR are already deploying Mako systems for mine countermeasures and persistent surveillance. Our $25,000 attritable units eliminate the need for expensive support vessels while delivering real-time intelligence at 10x lower cost than legacy systems. See how dual-domain autonomy can transform your operational capabilities within current budget constraints."
	imageSrc="/generated/image-a-naval-officer-in-technical-workwear-st.webp"
	callsToAction={[
		{
			href: "/contact",
			label: "Schedule a briefing",
			variant: "primary"
		},
		{
			href: "/about",
			label: "Learn about our technology",
			variant: "secondary"
		}
	]}
/>
