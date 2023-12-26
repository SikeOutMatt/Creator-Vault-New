<script>
    /** @type {import('./$types').PageData} */
    export let data;
    let videoTitle = "AP Sett One Shots";
</script>

<main class="mx-10">
    <div class="grid grid-cols-2">
        <div>
            <h1 class="text-2xl font-black py-1 text-[#2491eb]"> VIdeo Details </h1>
            <hr> 
            <div class="w-4/4">
                <div class="flex flex-col">
                    <label class="text-xl font-bold pt-3 text-[#2491eb]" for="title"> Title </label>
                    <input type="text" class="border border-black w-3/4" placeholder={videoTitle}> 
                </div>
                <div class="flex flex-col">
                    <label class="text-xl font-bold pt-3 text-[#2491eb]" for="description"> Description </label>
                    <textarea class="border border-black w-3/4" placeholder="This video is my craziest video yet you will not want to miss this. If you like this video then you will love the next one I have coming out" rows="4"></textarea>
                </div>
                <div class="flex flex-col">
                    <label class="text-xl font-bold pt-3 text-[#2491eb]" for="description"> Thumbnail </label>
                    <input type="file" class=" w-3/4">
                </div>

                <div class="flex flex-col">
                    <label class="text-xl font-bold pt-3 text-[#2491eb]" for="length"> Price </label>
                    <input type="text" class="border border-black w-3/4" placeholder="49.99">
                </div>
            </div>
        </div>
        <div>
            <h1> Other </h1>
        </div>
    </div>

</main>