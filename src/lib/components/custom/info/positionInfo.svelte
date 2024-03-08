<script>
  import LogoRound from "@/assets/SVGs/logoRound.svelte";
  import Link from "@/assets/SVGs/positionInfo/link.svelte";
  import ThreeDots from "@/assets/SVGs/positionInfo/threeDots.svelte";
  import Button from "@/components/ui/button/button.svelte";
  import * as Dropdown from "@/components/ui/dropdown-menu";
  import { Root } from "postcss";
</script>

<section class="flex flex-col items-end justify-between h-full">
  <section class="flex flex-col items-end justify-between">
    <LogoRound />
    <span class="font-bold text-xl">Duggup</span>
    <span class="text-[#7A9299] font-medium text-xs">Co-Founder and CEO</span>
  </section>
  <section class="flex items-center justify-between gap-2">
    <Button
      class="flex items-center gap-1 px-1 py-0.5"
      variant="ghost"
      href="https://drive.google.com/file/d/1mlF2Ed578KnMliXdw7wbHRqJWwFmcLMS/view?usp=sharing"
      target="_blank"
    >
      My website
      <Link />
    </Button>
    <Dropdown.Root>
      <Dropdown.Trigger>
        <Button variant="ghost" class="rounded-full p-1 px-2">
          <ThreeDots />
        </Button>
      </Dropdown.Trigger>
      <Dropdown.Content>
        <Dropdown.Label>Section 1</Dropdown.Label>
        <Dropdown.Group>
          <Dropdown.Item>Option 1</Dropdown.Item>
          <Dropdown.Item>Option 2</Dropdown.Item>
        </Dropdown.Group>
        <Dropdown.Separator />
        <Dropdown.Label>Section 2</Dropdown.Label>
        <Dropdown.Group>
          <Dropdown.Item>Option 3</Dropdown.Item>
          <Dropdown.Item>Option 4</Dropdown.Item>
        </Dropdown.Group>
      </Dropdown.Content>
    </Dropdown.Root>
  </section>
</section>
