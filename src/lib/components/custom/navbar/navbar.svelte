<script lang="ts">
  import Banner from "@/assets/SVGs/banner.svelte";
  import Logo from "@/assets/SVGs/logo.svelte";
  import Button from "../../ui/button/button.svelte";
  import NavBtns from "./navBtns.svelte";
  import Plus from "@/assets/SVGs/plus.svelte";
</script>

<navbar class="w-full flex items-center p-4 justify-between min-h-[73px]">
  <section class="flex items-center justify-center gap-2">
    <Logo />
    <Banner height="" width="" />
  </section>
  <section
    class="flex flex-col md:flex-row items-center justify-between w-[749px] h-[52px] gap-[40px]"
  >
    <section class="w-[461px] flex items-center justify-between">
      <NavBtns />
      <Button variant="outline" class="flex items-center gap-2">
        <Plus />
        <span>Post</span>
      </Button>
    </section>
  </section>
</navbar>
