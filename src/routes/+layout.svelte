<script>
  import "../app.postcss";
  import "../style.css";
  import Appbar from "$lib/Appbar.svelte";
  import Loader from "$lib/loader.svelte";
</script>

<Appbar />

<Loader />
<!-- page loader -->
<slot />
