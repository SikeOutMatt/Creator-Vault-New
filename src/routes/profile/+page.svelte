<script>
import Header from "../../components/header.svelte";
import Footer from '../../components/footer.svelte';
import thumbnail from "../../lib/assets/thumbnail.webp";
import profilebanner from "../../lib/assets/profilebanner.png";
import xlogo from "../../lib/assets/x-twitter.svg";
import instagram from "../../lib/assets/instagram.png";
import oflogo from "../../lib/assets/ofLogo.png";
import profllepic from "../../lib/assets/profilepic.jpeg";
import bunnyPic from '../../lib/assets/bunnypic.jpeg'
import videoThumnail from '../../lib/assets/videothumbnail.png'
import Videocard from "../../components/videocard.svelte";


function videoCard() {
    
}

let userTitle = "BunnyFuFuu's Vault";

    /** @type {import('./$types').PageData} */
    export let data;
</script>

<main>
    <Header />
    <div>
            <div class="mt-5">
                <section class="w-4/5 mx-auto bg-gray-100 rounded-md">
                    <div class="flex justify-center w-full">
                        <img class="rounded-md w-full max-h-48 object-fill" src={profilebanner} alt="Banner">
                    </div>
                    <div>
                        <img src={bunnyPic} alt="profilepic" class="rounded-full w-40 h-30 mx-auto -mt-20 object-fill">
                    </div>
                    <div class="flex flex-col justify-start items-center">
                        <h1 class="text-2xl sm:text-4xl font-bold"> BunnyFuFuu's Vault </h1>
                    </div>
                    <div class="flex justify-center items-center">
                        <h5 class="text-lg sm:text-xl font-semibold"> @BunnyFuFuu </h5>
                    </div>
                    <div class="flex justify-center items-center pb-5">
                        <img class="mx-2" src={xlogo} height="30px" width="30px" alt="x logo" > 
                        <img class="mx-2" src={instagram} height="30px" width="30px" alt="instagram logo"> 
                        <img class="mx-2" src={oflogo} height="30px" width="30px" alt="OF logo">
                    </div>
                </section>

                <div class=" w-4/5 mx-auto grid sm-grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-3 pt-8">
                    <div class="bg-[#2a2a2a] bg-opacity-10 rounded-xl cursor-pointer"> 
                        <img class="rounded-t-xl" src={videoThumnail} alt="thumbnail" width="100%" height="100%">
                        <div class="px-2">
                            <h1 class="font-bold text-2xl text-[#3d6c9d] py-2 "> Video Title </h1>
                            <div class="flex justify-between">
                                <p class="text-[#769fca] line-clamp-2 py-1"> This video is my craziest video yet you will not want to miss this. If you like this video then you will love the next one I have coming out </p>
                            </div>
                            <div class="flex justify-between pb-2">
                                <p class="text-[#769fca] font-semibold"> 6:12 </p>
                                <h4 class="text-[#769fca] font-semibold"> Price: $49.99 </h4>
                            </div>
                        </div>
                    </div>
                    <div class="bg-[#2a2a2a] bg-opacity-10 rounded-xl"> 
                        <img class="rounded-t-xl" src={videoThumnail} alt="thumbnail" width="100%" height="100%">
                        <div class="px-2">
                            <h1 class="font-bold text-2xl text-[#3d6c9d] py-2"> Video Title </h1>
                            <div class="flex justify-between">
                                <p class="text-[#769fca] line-clamp-2 py-1"> This video is my craziest video yet you will not want to miss this. If you like this video then you will love the next one I have coming out </p>
                            </div>
                            <div class="flex justify-between pb-2">
                                <p class="text-[#769fca] font-semibold"> 6:12 </p>
                                <h4 class="text-[#769fca] font-semibold"> Price: $49.99 </h4>
                            </div>
                        </div>
                    </div>
                    <div class="bg-[#2a2a2a] bg-opacity-10 rounded-xl"> 
                        <img class="rounded-t-xl" src={videoThumnail} alt="thumbnail" width="100%" height="100%">
                        <div class="px-2">
                            <h1 class="font-bold text-2xl text-[#3d6c9d] py-2"> Video Title </h1>
                            <div class="flex justify-between">
                                <p class="text-[#769fca] line-clamp-2 py-1"> This video is my craziest video yet you will not want to miss this. If you like this video then you will love the next one I have coming out </p>
                            </div>
                            <div class="flex justify-between pb-2">
                                <p class="text-[#769fca] font-semibold"> 6:12 </p>
                                <h4 class="text-[#769fca] font-semibold"> Price: $49.99 </h4>
                            </div>
                        </div>
                    </div>
                 
             

                    
                    
            

                 
                </div>
                
            </div>
        </div>
<Footer />




</main>