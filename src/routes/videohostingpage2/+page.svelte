<script>
    import Header from '../../components/header.svelte';
    import Footer from '../../components/footer.svelte';
    /** @type {import('./$types').PageData} */
    export let data;
</script>


<main>
<Header />
 
    <div class="flex justify-center items-center h-[500px] w-3/4 mx-auto mt-8">
        <iframe
          src="https://customer-p305r8zuikgo2oi9.cloudflarestream.com/22d65e330136f7bc1a58f3f4372758e9/iframe?poster=https%3A%2F%2Fcustomer-p305r8zuikgo2oi9.cloudflarestream.com%2F22d65e330136f7bc1a58f3f4372758e9%2Fthumbnails%2Fthumbnail.jpg%3Ftime%3D%26height%3D600"
          style="border: none; top: 0; left: 0; height: 100%; width: 70%;"
          allow="accelerometer; gyroscope; autoplay; encrypted-media; picture-in-picture;"
          allowfullscreen="true"
        ></iframe>
      </div>
      <div class="w-3/4 mx-auto flex justify-center items-start pt-4">
        <button class="bg-black rounded-lg font-bold text-white text-2xl p-2"> Purchase Now for $49.99</button>
      </div>

<Footer />
</main>