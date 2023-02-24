<script>
  import "../app.postcss";
  import Appbar from "$lib/Appbar.svelte";
    import Leftbar from "$lib/leftbar.svelte";
    import RightBar from "$lib/rightBar.svelte";
  // import Loader from "$lib/loader.svelte";
</script>

<Appbar />

<!-- page start -->
<div class="page-body container-fluid custom-padding profile-page">
  <Leftbar />
  <!-- <Loader /> -->
  <!-- page loader -->
  <slot />
  <RightBar />
</div>
  