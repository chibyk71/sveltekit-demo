<script>
  import "../../app.postcss";
  import Appbar from "$lib/Appbar.svelte";
  import Leftbar from "$lib/leftbar.svelte";
  import RightBar from "$lib/rightBar.svelte";
</script>
<Appbar />

<!-- page start -->
<div class="page-body container-fluid custom-padding">
  <Leftbar />
  <div class="page-center">
    <slot />
  </div>
    <RightBar />
</div>
  