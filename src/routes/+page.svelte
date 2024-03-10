<script>
  import TimelineV1 from "./sections/timelineV1.svelte";
  import TimelineV2 from "./sections/timelineV2.svelte";
  import ProfileSection from "./sections/profileSection.svelte";
  import { data1 } from "../lib/data";
  import { data2 } from "../lib/data";
</script>

<div
  class="flex flex-col flex-1 justify-center pb-10 md:pb-14 max-w-[1400px] m-auto mt-10"
>
  <!-- Profile Section -->
  <ProfileSection />

  <!-- Experience Section -->
  <TimelineV1 date="Dec 2023" cardData={data1} />
  <!-- Another experience section -->
  <TimelineV2
    companyName="Duggup"
    location="San Francisco Bay Area"
    date="Nov 2023"
    logo="/icons/logo-cir.svg"
  />
  <!-- Third Experience section -->
  <TimelineV1 date="Dec 2023" cardData={data2} />

  <TimelineV2
    companyName="BetterUp"
    location="San Francisco Bay Area"
    date="Nov 2023"
    logo="/icons/better-up.svg"
  />
</div>
