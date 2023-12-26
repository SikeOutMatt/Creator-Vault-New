<script>
      let username = "BunnyFuFuu"
    let user_id = "@BunnyFuFuu"
    import profilePicture from '../../lib/assets/bunnypic.jpeg'
    import backIcon from '../../lib/assets/back.png'


function toggleSidebar() {
    let sidebar = document.getElementById("sidebarSection")
    let backIcon = document.getElementById("backIcon")
    if (sidebar.classList.contains("hidden")) {
        sidebar.classList.remove("hidden")
        backIcon.classList.add("rotate-180")
    } else {
        sidebar.classList.add("hidden")
        backIcon.classList.remove("rotate-180")
    }
}

</script>

<section>
    <section class="pl-6 bg-[#2491eb] bg-opacity-20 h-full rounded-r-lg pt-5 sm:block hidden">
        <div class="flex items-center justify-start">
         <img class="rounded-full mr-3" height="50" width="50" src={profilePicture} alt="profile picture" >
         <div class="flex flex-col">
                <h1 class="text-xl font-bold"> {username}</h1>
                <h6 class="text-sm"> {user_id} </h6>
         </div>
         <img id="backIcon" on:click={toggleSidebar} class="ml-2" src={backIcon} alt="back icon" width="20" height="20">
     </div>
    
     <section>
         <div class="pt-5"> 
                <a href="/dashboard" ><button class=" text-left w-full rounded-md font-bold p-1 my-1"> Overview </button> </a>
                <a href="/dashboard/videos"><button class=" text-left w-full rounded-md font-bold p-1 my-1"> My Videos </button> </a>
             <a href="/dashboard/payouts"><button class="text-left w-full rounded-md font-bold p-1 my-1"> Payouts  </button> </a>
                <a href="/dashboard/purchases"> <button class="text-left w-full rounded-md font-bold p-1 my-1"> Purchases  </button> </a>
                <a href="/dashboard/payment"> <button class="text-left w-full rounded-md font-bold p-1 my-1"> Payment  </button> </a>
            </div>
        </section>
    </section>
</section>