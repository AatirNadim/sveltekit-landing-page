<script>
  import Navbar from "@/components/custom/navbar/navbar.svelte";
  import "../app.pcss";
  import InfoWrapper from "@/components/custom/info/infoWrapper.svelte";
  import MainTimeline from "@/components/custom/timeline/mainTimeline.svelte";
  
</script>

<body class="flex flex-col items-center" >
  <section class="w-full max-w-[1424px] flex flex-col items-center overflow-auto gap-4">
    <Navbar />
    <InfoWrapper />
    <MainTimeline />
    <!-- <footer class="w-full">
      <slot name="footer">this is the default footer</slot>
    </footer> -->
  </section>
</body>
