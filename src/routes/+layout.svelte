<script>
  import "../app.postcss";
  import Appbar from "$lib/Appbar.svelte";
  import Loader from "$lib/loader.svelte";
</script>

<Appbar />

<Loader />
<!-- page loader -->
<slot />
