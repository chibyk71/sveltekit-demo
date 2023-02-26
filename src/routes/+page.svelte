<script>
  import Birthday from "$lib/component/sidebar/birthday.svelte";
  import EventInvite from "$lib/component/sidebar/eventInvite.svelte";
  import Invitation from "$lib/component/sidebar/invitation.svelte";
  import ProfileBox from "$lib/component/sidebar/profileBox.svelte";
  import SideGalery from "$lib/component/sidebar/sideGalery.svelte";
  import SuggesionBox from "$lib/component/sidebar/suggesionBox.svelte";
  import Weather from "$lib/component/sidebar/weather.svelte";

</script>
<div class="content-left">
    <SideGalery />
    <Birthday />
    <Invitation />
    <EventInvite />
    
    <Weather />
    
    <ProfileBox />

    <SuggesionBox />
</div>