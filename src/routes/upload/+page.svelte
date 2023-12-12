<script>
    import Header from "../../components/header.svelte";
    import Footer from "../../components/footer.svelte";
    /** @type {import('./$types').PageData} */
    export let data;
</script>


<main>
    <Header />
    <div class="w-4/5 mx-auto">
        <div>
            <h1 class="font-bold text-2xl mt-8"> Upload Your Content </h1>
            <p> Upload your content to Creator Vault </p>
            <hr class="h-px my-8 bg-gray-200 border-0 dark:bg-gray-700">
        </div> 
        <div class="grid md:grid-cols-3 grid-cols-1 ">
            <form class="pt-1"> 
                <div class="flex flex-col">
                     <label class="text-2xl font-bold" for="videoTitle"> Video Title </label>
                     <input class="border py-1 border-gray-500 sm:w-full " type="text" placeholder="Video Title"> 
             </div>
            <div class="flex flex-col mt-7">
                <label class="text-2xl font-bold"> Upload File </label>
                <input type="file" name="file" id="file" class=""  />
            </div>
            <div class="flex flex-col mt-7">
                <label class="text-2xl font-bold" for="videoDescription"> Video Description </label>
                <textarea class="border py-1 border-gray-500  resize-none sm:w-full " name="videoDescription" id="videoDescription" cols="30" rows="4" placeholder="Video Description"></textarea>
            </div>
            <div class="flex flex-col mt-7">
                <label class="text-2xl font-bold"> Upload Thumbnail </label>
                <input type="file" name="file" id="file" class=""  />
            </div>
            <div class="flex flex-col mt-7">
                <label class="text-2xl font-bold" for="videoTitle"> Price </label>
                <input class="border py-1 border-gray-500 sm:w-full " type="text" placeholder="Video Price (In USD)"> 
            </div>
            <div class="mt-7 flex justify-center items-center">
                <button class="text-lg font-bold bg-black text-white mx-3 p-2 rounded-md"> Upload </button>
                <button class="text-lg font-bold bg-black text-white p-2 rounded-md mx-3"> Discard </button>

            </div>

             </form>
    <div class="flex justify-center col-span-2 items-center">
        <div class="bg-gray-100 sm:h-3/4 sm:w-3/4 h-full w-full py-10 flex items-center justify-center">
            <h1 class="text-2xl font-bold"> Video Preview</h1>

        </div>
    </div>

    </div>
       





    </div>






    <Footer />
</main>