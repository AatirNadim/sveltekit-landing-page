<script>
  import LogoRound from "@/assets/SVGs/logoRound.svelte";
  import Link from "@/assets/SVGs/positionInfo/link.svelte";
  import ThreeDots from "@/assets/SVGs/positionInfo/threeDots.svelte";
</script>

<section class="flex flex-col items-end justify-between h-full">
  <section class="flex flex-col items-end justify-between">
    <LogoRound />
    <span class="font-bold text-xl">Duggup</span>
    <span class="text-[#7A9299] font-medium text-xs">Co-Founder and CEO</span>
  </section>
  <section class="flex items-center justify-between gap-4">
    <span class="flex items-center gap-1">
      My website
      <Link />
    </span>
    <ThreeDots />
  </section>
</section>
