<script lang="ts">
    export let title: string;
    export let link: string;
    export let image: string;
</script>

<div class="card card-compact bg-base-100 w-96 shadow-xl m-3">
    <figure>
        <img
            src="{image}"
            alt="{title}"
            class="aspect-square object-contain"
        />
    </figure>
    <div class="card-body">
        <h2 class="card-title">{title}</h2>
        <div class="card-actions justify-end">
            <a href="{link}" target="_blank" class="btn btn-primary">Learn more</a>
        </div>
    </div>
</div>