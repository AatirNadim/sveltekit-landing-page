<script lang="ts">
  import { Timeline, TimelineItem, Button } from "flowbite-svelte";
  // import { ArrowRightOutline } from 'flowbite-svelte-icons';
  import Jobbs from "@/assets/PNGs/jobbs.jpeg";
  import Altman from "@/assets/PNGs/altman.jpeg";
  import Setup from "@/assets/PNGs/system_setup.jpeg";
  import Map from "@/assets/PNGs/map.png";
  import CardWrapper from "./card/cardWrapper.svelte";
  import LogoRound from "@/assets/SVGs/logoRound.svelte";
  import BetterUp from "@/assets/PNGs/betterup.jpeg"
</script>

<Timeline order="default">
  <TimelineItem
    classLi="relative flex gap-4 justify-evenly w-[780px] ms-6 mt-4"
    classDiv="top-1/2 left-[-30px] bg-white border-2 border-[#0066FF]"
  >
    <CardWrapper
      imgUrl={Jobbs}
      text={"No amount of technology can convert a bad story into a good story."}
    />
    <CardWrapper
      imgUrl={Altman}
      text={"Most people don't have original ideas. Here is how Sam Altman pushes himself to have unpopular ideas."}
    />
  </TimelineItem>
  <TimelineItem
    classLi="relative bg-white flex flex-col p-4 ms-6"
    classDiv="top-1/2 left-[-36px] bg-white border-[6px] border-[#0066FF] w-6 h-6"
  >
    <section class="absolute left-[-210px] top-[-10px] flex flex-col items-end text-sm" >
      <LogoRound size="48" />
      <div class="text-[#7A9299] mt-2" >San Francisco Bay Area</div>
      <div class="text-[#7A9299]" >Joined</div>
      <div class="text-[#7A9299]" >Nov 2023</div>
    </section>
    <span class="font-bold text-xl">Co-Founder and CEO</span>
    <span class="font-light text-[##7A9299] flex items-center gap-1"
      >Full-time · Remote</span
    >
  </TimelineItem>
  <TimelineItem
    classLi="relative flex gap-4 justify-evenly ms-6"
    classDiv="top-1/2 left-[-30px] bg-white border-2 border-[#0066FF]"
  >
    <CardWrapper
      imgUrl={Setup}
      text={`Startup Lesson I am reflecting. Don't build for the "average person".`}
    />
    <CardWrapper
      imgUrl={Map}
      text={"Your biggest regrets at 80 will be acts of omission."}
    />
  </TimelineItem>
  <TimelineItem
    classLi="relative bg-white flex flex-col p-4 ms-6"
    classDiv="top-1/2 left-[-36px] bg-white border-[6px] border-[#0066FF] w-6 h-6"
  >
  <section class="absolute left-[-210px] top-[-10px] flex flex-col items-end text-sm" >
    <img src={BetterUp} alt="Betterup" class="h-[48px] rounded-full mb-2" />
    <div class="text-[#7A9299]" >San Francisco Bay Area</div>
    <div class="text-[#7A9299]" >Joined</div>
    <div class="text-[#7A9299]" >Nov 2023</div>
  </section>
    <span class="font-bold text-xl">VP Engineering</span>
    <span class="font-light text-[##7A9299]">Full-time</span>
  </TimelineItem>
</Timeline>
