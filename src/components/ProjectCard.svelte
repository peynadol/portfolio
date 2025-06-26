<script lang="ts">
  export let title: string;
  export let description: string;
  export let tech: string[] = [];
  export let live: string;
  export let github: string;
  export let image: string | undefined;
</script>

<div class=" rounded-xl p-6 hover:bg-muted/10 transition">
  {#if image}
    <img
      src={image}
      alt="{title} screenshot"
      class="rounded-md mb-4 border border-muted shadow-sm"
    />
  {/if}

  <h3 class="text-xl font-semibold mb-2">{title}</h3>
  <p class="text-muted mb-4">{description}</p>

  <ul class="flex flex-wrap gap-2 text-sm mb-4">
    {#each tech as item}
      <li class="px-2 py-1 bg-muted text-muted-foreground rounded">{item}</li>
    {/each}
  </ul>

  <div class="flex gap-4 text-sm">
    <a href={live} class="text-accent hover:underline" target="_blank"
      >Live Site</a
    >
    <a href={github} class="text-accent hover:underline" target="_blank"
      >GitHub</a
    >
  </div>
</div>
