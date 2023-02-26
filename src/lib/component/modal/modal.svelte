<script>
    import { fade } from "svelte/transition";
    export let show = false;
    export let cls = "";
</script>
{#if show}
<div transition:fade class="{cls} modal fade mobile-full-width show" tabindex="-1" aria-labelledby="modal-header" 
aria-modal="true" role="dialog">
    <div class="modal-dialog modal-dialog-centered" role="document">
        <div class="modal-content share-modal">
            <div class="modal-header">
                <slot name="header" />
            </div>
            <div class="modal-body">
                <slot name="body" />
            </div>
            <div class="modal-footer">
                <slot name="footer"><!-- optional fallback --></slot>
            </div>
        </div>
    </div>
</div> 
{/if}     