<script lang="ts">
	import { Announcement, ThemeCustomizer, ThemeWrapper } from "$lib/components/docs/index.js";
	import * as PageHeader from "$lib/components/docs/page-header/index.js";
	import { CardsNewYork } from "$lib/registry/new-york/example/cards/index.js";
	import { CardsDefault } from "$lib/registry/default/example/cards/index.js";
	import { config } from "$lib/stores/index.js";
	import Dashboard_01 from "$lib/registry/default/block/dashboard-01.svelte";
	import Dashboard_02 from "$lib/registry/default/block/dashboard-02.svelte";
	import Dashboard_03 from "$lib/registry/default/block/dashboard-03.svelte";
	import Dashboard_04 from "$lib/registry/default/block/dashboard-04.svelte";
	import Dashboard_05 from "$lib/registry/default/block/dashboard-05.svelte";
	import Dashboard_06 from "$lib/registry/default/block/dashboard-06.svelte";
	import Dashboard_07 from "$lib/registry/default/block/dashboard-07.svelte";
</script>

<svelte:head>
	<style>
		@import "/registry/themes.css";
		:root {
			--vis-color0: var(--primary);
			--vis-color1: #ffffff;
			--vis-color2: #ffffff;
			--vis-color3: #ffffff;
			--vis-color4: #ffffff;
		}
	</style>
</svelte:head>

<div class="container pt-20">
	<!-- <ThemeWrapper
		
		class="relative flex flex-col items-start md:flex-row md:items-center"
	>
		<PageHeader.Root>
			<Announcement />
			<PageHeader.Heading class="hidden md:block">
				Add colors. Make it yours.
			</PageHeader.Heading>
			<PageHeader.Heading class="md:hidden">Make it yours.</PageHeader.Heading>
			<PageHeader.Description balanced={false}>
				Hand-picked themes that you can copy and paste into your apps.
			</PageHeader.Description>
			<div class="flex w-full items-center justify-center space-x-4 py-4 md:pb-10">
				<ThemeCustomizer />
			</div>
		</PageHeader.Root>
	</ThemeWrapper> -->
	<ThemeWrapper>
		<!-- {#if $config.style === "new-york"}
			<CardsNewYork />
		{:else}
			<CardsDefault />
		{/if} -->
		<CardsDefault />
		<!-- <div class="-mx-14 pt-8">
			<Dashboard_01/>
			<Dashboard_02/>
			<Dashboard_04/>
		</div>

		<Dashboard_03/> -->
		
		
		<!-- <Dashboard_05/> -->
		<!-- <Dashboard_06/> -->
		<!-- <Dashboard_07/> -->
	</ThemeWrapper>
</div>
