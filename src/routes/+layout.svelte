<script lang="ts">
  import "../app.css";
  import { Toaster } from "svelte-5-french-toast";
</script>

<svelte:head>
  <title>Liam Peynado – Portfolio</title>
</svelte:head>

<main class="min-h-screen bg-background text-foreground">
  <div class="px-6 md:px-8 max-w-4xl mx-auto">
    <slot />
    <Toaster position="bottom-right" />
  </div>
</main>
