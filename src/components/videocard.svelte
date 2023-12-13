<script>

export let showVideocard = false;

let toggleVideoCard = () => {
    showVideocard = !showVideocard;
};



</script>


{#if showVideocard}
<main class="flex justify-center items-center fixed h-screen w-screen bg-black bg-opacity-40">
    <div class=" w-3/4 sm:w-2/4 mx-auto bg-[#f7fbfc] rounded-xl">
        <div class="grid grid-cols-1 sm:grid-cols-2">
            <div class=" flex justify-center items-center">
                <div class="bg-slate-400 h-3/4 w-3/4 flex items-center justify-center">
                    <h1 class="text-xl font-bold"> Video Preview</h1>
                </div>
            </div>
            <div class="pr-5">
                <h1 class="text-4xl font-bold py-2"> AP Sett One Shots </h1>
                <p class="pt-2 pb-1"> This video is my craziest video yet you will not want to miss this. If you like this video then you will love the next one I have coming out </p>
                <h3 class="py-1"><strong> Length:</strong> 6:12 </h3>
                <h3 class="py-1"> <strong> Price: </strong>  $49.99 </h3>

                <div class=" py-5 flex justify-around">
                    <a href="/checkout"> <button class="bg-[#2a2a2a] text-[#f7fbfc] font-bold  p-3 rounded-md"> Purchase</button> </a>
                    <button on:click={toggleVideoCard}> Cancel </button>
                </div>
            </div>
        </div>
    </div>
</main>
{/if}
