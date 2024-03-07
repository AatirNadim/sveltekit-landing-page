<script>
  import Navbar from "@/components/custom/navbar/navbar.svelte";
  import "../app.pcss";
  
</script>

<body class="flex flex-col items-center w-screen" >
  <section class="w-full max-w-[1424px] flex flex-col overflow-auto">
    <Navbar />
    <footer class="w-full">
      <slot name="footer">this is the default footer</slot>
    </footer>
  </section>
</body>
