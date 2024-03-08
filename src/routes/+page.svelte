<script>
  import TimelineV1 from "./sections/timelineV1.svelte";
  import TimelineV2 from "./sections/timelineV2.svelte";
  import ProfileSection from "./sections/profileSection.svelte";
</script>

<div
  class="flex flex-col flex-1 justify-center pb-10 md:pb-14 max-w-[1400px] m-auto mt-10"
>
  <!-- Profile Section -->
  <ProfileSection />

  <!-- Experience Section -->
  <TimelineV1 />
  <!-- Another experience section -->
  <TimelineV2 />
  <!-- Third Experience section -->
  <TimelineV1 />

  <TimelineV2 />
</div>
