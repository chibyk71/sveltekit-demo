  <script>
	import { onMount } from 'svelte';
    export let loaded = false;

    onMount(() => setTimeout(()=>loaded = true, 1500));
  </script>
  
  <!-- content here -->
  <div class="page-loader" class:hidden={loaded}>
    <div class="loader">
      <span class="loader-item" /><span class="loader-item" /><span
        class="loader-item"
      /><span class="loader-item" /><span class="loader-item" /><span
        class="loader-item"
      /><span class="loader-item" /><span class="loader-item" /><span
        class="loader-item"
      /><span class="loader-item" />
    </div>
  </div>