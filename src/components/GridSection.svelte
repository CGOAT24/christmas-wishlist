<script lang="ts">
    import GridItem from "./GridItem.svelte";

    export let category: string = "General";
    export let items: {title: string, link: string, image: string, category: string | undefined}[];
</script>
<div class="flex flex-col w-full m-3 rounded-lg bg-base-200">
    <div class="h-full w-full">
        <h1 class="text-3xl font-bold mt-3 ml-3">{category}</h1>
    </div>
    <div class="flex justify-evenly items-center flex-wrap w-full h-full">
        {#each items as item}
            <GridItem title={item.title} link={item.link} image={item.image} />
        {/each}
    </div>
</div>
