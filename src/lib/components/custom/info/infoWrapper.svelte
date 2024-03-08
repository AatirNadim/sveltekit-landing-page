<script lang="ts" >
  import Person from "@/assets/PNGs/person.jpeg"
  import InfoText from "./infoText.svelte";
  import PositionInfo from "./positionInfo.svelte";
</script>

<section  class="w-full md:w-4/5 flex flex-col md:flex-row items-center justify-between" >
  <div class="flex flex-col gap-1 items-center" >
    <img src={Person} class="w-[120px] h-[120px] rounded-full" alt="person" />
    <span class="text-[#4B5C6D] font-bold text-2xl" >
      Krishna Kiran
    </span>
  </div>
  <section class="w-full max-w-[834px] flex flex-col md:flex-row items-center md:justify-between md:h-[138px]" >
    <InfoText />
    <PositionInfo />
  </section>
</section>