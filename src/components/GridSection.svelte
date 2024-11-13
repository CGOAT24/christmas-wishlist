<script lang="ts">
    import GridItem from "./GridItem.svelte";

    export let category: string = "General";
    export let items: {title: string, link: string, image: string, category: string | undefined}[];
</script>
<div class="divide-y w-full">
    <h2 class="text-left m-3 w-full">{category}</h2>
    <div class="flex justify-between items-center flex-wrap w-full h-full">
        {#each items as item}
            <GridItem title={item.title} link={item.link} image={item.image} />
        {/each}
    </div>

</div>
