<script lang="ts" >
  import Home from "@/assets/SVGs/navbar/home.svelte";
  import Learn from "@/assets/SVGs/navbar/learn.svelte";
  import Story from "@/assets/SVGs/navbar/story.svelte";
  import Button from "@/components/ui/button/button.svelte";

  
</script>

<section class="w-[319px] flex items-center justify-between">
  <Button variant="ghost" class="flex gap-2">
    <Home />
    <span>Home</span>
  </Button>
  <Button variant="ghost" class="flex gap-2">
    <Story />
    <span>Explore</span>
  </Button>
  <Button variant="ghost" class="flex gap-2">
    <Learn />
    <span>Learn</span>
  </Button>
</section>