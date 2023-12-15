<script>
    /** @type {import('./$types').PageData} */
    export let data;
    import videoThumbnail from '../../../lib/assets/videothumbnail.png'
</script>

<main class=" mx-10">
    <section>
        <div class="flex justify-between">
            <h1 class="text-2xl font-black py-1 text-[#2491eb]"> Your Videos </h1>
            <h6> Filters </h6>

        </div>
        <div class="py-4 grid grid-cols-1 gap-3 md:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 ">
           <a href="/dashboard/videos/ap-sett-one-shot"> <div class=" shadow-xl hover:shadow-2xl bg-slate-200 ">
                <img class=" rounded-t-md" src={videoThumbnail}>
                <div class="p-2">
                    <h1 class="text-lg text-[#2491eb] font-bold z-10"> AP Sett One-Shots</h1>
                    <p class="text-sm"> Uploaded On: 12/14/2023</p>
                </div>
            </div> </a>
            <div class=" shadow-xl hover:shadow-2xl bg-slate-200 ">
                <img class=" rounded-t-md" src={videoThumbnail}>
                <div class="p-2">
                    <h1 class="text-lg text-[#2491eb] font-bold z-10"> AP Sett One-Shots</h1>
                    <p class="text-sm"> Uploaded On: 12/14/2023</p>
                </div>
            </div>
            <div class=" shadow-xl hover:shadow-2xl bg-slate-200 ">
                <img class=" rounded-t-md" src={videoThumbnail}>
                <div class="p-2">
                    <h1 class="text-lg text-[#2491eb] font-bold z-10"> AP Sett One-Shots</h1>
                    <p class="text-sm"> Uploaded On: 12/14/2023</p>
                </div>
            </div>
            <div class=" shadow-xl hover:shadow-2xl bg-slate-200 ">
                <img class=" rounded-t-md" src={videoThumbnail}>
                <div class="p-2">
                    <h1 class="text-lg text-[#2491eb] font-bold z-10"> AP Sett One-Shots</h1>
                    <p class="text-sm"> Uploaded On: 12/14/2023</p>
                </div>
            </div>
           

        </div>
    </section>
</main>