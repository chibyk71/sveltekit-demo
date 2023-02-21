
<script>
  import {Button} from 'flowbite-svelte';
</script>
<div class="container bg-blue-500">
  <div class="fixed flex gap-2 justify-between items-center py-1 min-w-full px-2 md:hidden">
    <div class="logo res w-5/12">
      <img src="images/logo.png" alt="logo" />
      <span>Socimo</span>
    </div>
    <div class="user-avatar mobile w-4/12 self-center">
      <a href="profile.html" title="View Profile" ><img alt="" src="images/resources/user.jpg" /></a>
    </div>
    <Button pill={true} outline={true} class="w-1/12" size="md"><i class="fas fa-search"></i></Button>
    <Button pill={true} outline={true} class="w-1/12" size="md"><span class="fas fa-moon font-normal"></span></Button>  
  </div>
</div>

