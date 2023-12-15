<script>
    import Sidebar from "./sidebar.svelte";
    

  </script>


<main class="flex mt-4">
  <div class="w-1/6 ">
    <Sidebar />
  </div>
 <div class="w-full">
    <slot />
 </div>
</main>
