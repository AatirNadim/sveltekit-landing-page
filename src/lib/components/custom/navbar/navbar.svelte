<script lang="ts">
  import Banner from "@/assets/SVGs/banner.svelte";
  import Logo from "@/assets/SVGs/logo.svelte";
  import Button from "@/components/ui/button/button.svelte";
  import NavBtns from "./navBtns.svelte";
  import Person from "@/assets/PNGs/person.jpeg";
  import Plus from "@/assets/SVGs/plus.svelte";
  import ArrowDown from "@/assets/SVGs/navbar/arrowDown.svelte";
  import Dotted from "@/assets/SVGs/navbar/dotted.svelte";
  import * as Dropdown from "@/components/ui/dropdown-menu"
</script>

<div class="flex flex-col w-full mb-12">
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
        <Button
          variant="outline"
          class="flex items-center gap-2 border-b-4 border-black w-[102px]"
        >
          <Plus />
          <span>Post</span>
        </Button>
      </section>
      <section class="flex w-[248px] items-center justify-evenly">
        <img src={Person} alt="person" class="rounded-full w-[48px] h-[48px]" />
        <Dropdown.Root  >
          <Dropdown.Trigger  >
            <Button class="gap-1 justify-between " variant="ghost">
              <span class="text-[#4D4D4D] text-xl">Krishna Kiran</span>
              <ArrowDown />
            </Button>
          </Dropdown.Trigger>
          <Dropdown.Content  >
            <Dropdown.Label >Section 1</Dropdown.Label>
            <Dropdown.Group >
              <Dropdown.Item >Option 1</Dropdown.Item>
              <Dropdown.Item >Option 2</Dropdown.Item>
            </Dropdown.Group>
            <Dropdown.Separator />
            <Dropdown.Label >Section 2</Dropdown.Label>
            <Dropdown.Group >
              <Dropdown.Item >Option 3</Dropdown.Item>
              <Dropdown.Item >Option 4</Dropdown.Item>
            </Dropdown.Group>
          </Dropdown.Content>
        </Dropdown.Root>
        
      </section>
    </section>
  </navbar>
  <Dotted />
</div>
