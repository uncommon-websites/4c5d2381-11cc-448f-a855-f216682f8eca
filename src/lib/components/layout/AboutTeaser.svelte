<!--
@component AboutTeaser
A minimalist teaser for the about page.
-->
<script lang="ts">
	// Types
	type TeamMember = {
		name: string;
		role: string;
		image: string;
	};

	// Components
	import Button from "../ui/Button.svelte";
	import ScrollText from "./sub/ScrollText.svelte";

	// State
	let sectionRef: HTMLElement;

	let props = $props();

	// Data
	const teamMember: TeamMember = {
		name: "Founder & CEO",
		role: "Ulysses",
		image: "/generated/image-environmental-documentary-portrait-of-a-.webp"
	};
</script>

<section bind:this={sectionRef} {...props}>
	<div class="section-px section-py container mx-auto">
		<div class="relative mx-auto grid max-w-2xl place-items-center gap-16">
			<ScrollText
				class="text-title1 text-center"
				text={`"I watched a Navy diver spend six hours surveying a quarter-mile of seabed that our system now maps in twenty minutes. That's when I knew we weren't just building robots—we were giving humanity the tools to finally steward seventy percent of our planet."`}
			/>

			<!-- Team Member & CTA Section -->
			<div class="flex flex-col items-center gap-6 md:flex-row md:gap-8">
				<img
					src={teamMember.image}
					alt={teamMember.name}
					class="size-16 rounded-full object-cover border-2 border-gray-200"
				/>
				<div class="text-center md:text-left">
					<div class="text-callout font-medium">{teamMember.name}</div>
					<div class="text-caption text-muted-foreground">{teamMember.role}</div>
				</div>
				<Button href="/about" variant="secondary" size="sm" class="md:ml-auto">
					Read our story
				</Button>
			</div>
		</div>
	</div>
</section>
