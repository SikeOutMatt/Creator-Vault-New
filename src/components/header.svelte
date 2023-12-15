<script>
import Logo from '../lib/assets/creatorvaultlogo.png'
import Hamburer from '../lib/assets/hamburger.png'
import mobileLogo from '../lib/assets/CreatorVaultMobile.png'
import Sidebar from './sidebar.svelte'

function showSidebar() {
    let sidebar = document.getElementById("sidebar")

    if (sidebar.classList.contains("hidden") ) {
        sidebar.classList.remove("hidden");
    } else {
        sidebar.classList.add("hidden");
    };
};


</script> 

<main>
    <div class="w-10/12	mx-auto">
        <div class="flex justify-between items-baseline">
            <div>
                <div class="hidden md:flex">
                   <a href="/home"> <img src={Logo} alt="logo" width="250" height="200"> </a> 
                </div>
                <div class="flex md:hidden">
                   <a href="/home">  <img src={mobileLogo} alt="logo" width="75" height="75"></a>
                </div>

            </div>
            <div class>
                <nav class=""> 
                    <img on:click={showSidebar} class="md:hidden mt-10" src={Hamburer} width="30" height="30" alt="hamburger menu icon">
                    <ul class="hidden md:flex mt-10 items-center ">
                        <li class="px-2"> <a href="/home"> Home </a></li>
                        <li class="px-2 "><a href="/dashboard"> Dashboard</a> </li>
                        <li class="px-2"> <a href="/profile"> Profile </a>  </li>
                        <li class="px-2"> <a href="/account"> Account </a> </li>
                        <a href="/upload"> <button class="text-md font-bold p-2 bg-black rounded-md text-white"> Upload </button></a>
                    </ul>
                </nav>
            </div>
        </div>
    </div>
    <div class="hidden" id="sidebar">
        <Sidebar />
    </div>
</main>
