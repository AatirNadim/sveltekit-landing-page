<script lang="ts" >
  export let imgUrl : string = ""
  export let text = ""
</script>

<section class="overflow-hidden rounded-lg w-[334px] h-[226px] border-[0.5px] border-[#D0D5DD]" >
  <img src={imgUrl} alt="image" class="h-[136px] w-full object-cover" />
  <!-- <div class="flex items-center justify-center flex-1" > -->
  <span class="flex items-center justify-center text-sm h-[90px] px-4" >{text}</span>
<!-- </div> -->
</section>