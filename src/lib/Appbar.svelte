<script>
  import {Button} from 'flowbite-svelte';
  import { tweened } from "svelte/motion";
  let value = "";

  $: icon = (value?.trim() == "" && !value) ? true: false ;
 
  let searchBock = 100;
  const swidth = tweened(searchBock);
  $:swidth.set(searchBock);
  $:sc = ($swidth == 0)? "hidden": "";

  let handleClick = () => {
    searchBock = 0;
  }

</script>
<div class="fixed container bg-blue-500 w-full">
  <div style='width:{$swidth}%;' class="{sc} absolute left-0 top-0 bg-blue-500 w-full h-14 z-10 px-1 pt-1 overflow-hidden">
    <form class="flex gap-px justify-center items-center w-full">
      {#if icon}
         <!-- content here -->
         <button on:click={handleClick} class="uk-button uk-button-default"><i class="fas fa-times"></i></button>
      {:else}
         <!-- else content here -->
         <button type="submit" class="uk-button uk-button-default"><i class="fas fa-search"></i></button>`
      {/if}
      <!-- <Button pill={true} class="w-1/12  bg-transparent text-white" size="md"><span class="fas {icon}"></span></Button>   -->
      <input class="inline-block w-full" type="search" bind:value placeholder="" aria-label="">
    </form>
  </div>
  <div class="flex gap-2 max-h-28 justify-between items-center py-1 min-w-full px-2 md:hidden">
    <div class="logo res w-5/12">
      <img src="images/logo.png" alt="logo" />
      <span>Socimo</span>
    </div>
    <div class="user-avatar mobile w-4/12 self-center">
      <a href="profile.html" title="View Profile" ><img alt="" src="images/resources/user.jpg" /></a>
    </div>
    <Button pill={true} outline={true} on:click={() => searchBock = 100} class="w-1/12 bg-transparent text-white" size="md"><i class="fas fa-search"></i></Button>
    <Button pill={true} outline={true} class="w-1/12  bg-transparent text-white" size="md"><span class="fas fa-moon font-normal"></span></Button>  
  </div>
</div>

