<script>
  import Button from "@/components/ui/button/button.svelte";
  import { infoStr } from "@/constants";
</script>
<section class="w-4/5 flex flex-col items-start gap-4 h-full" >
  <span class="w-full text-wrap" >
    {infoStr}
  </span>
  <Button variant="ghost" class="border border-b-4 border-black w-[91px]" >
    Follow
  </Button>
</section>