<script>
import Header from "../../components/header.svelte";
import Footer from "../../components/footer.svelte";
import hamburger from "../../lib/assets/hamburger.png";
import {onMount} from "svelte";

    /** @type {import('./$types').PageData} */
    export let data;



    let pageTypeHeading = "";

    onMount(() => {
    let profileBtn = document.getElementById("profileBtn");
    let profileSection = document.getElementById("profileSection");
    let accountBtn = document.getElementById("accountBtn");
    let accountSection = document.getElementById("accountSection");

    profileBtn.addEventListener("click", function( ) {
        if (profileSection.classList.contains("hidden")) {
            profileSection.classList.remove("hidden");
            accountSection.classList.add("hidden");
            profileBtn.style.backgroundColor = "#DDDDDD";
            accountBtn.style.backgroundColor = "white";
        } else {
            profileSection.classList.remove("hidden");
        }
    });

    accountBtn.addEventListener("click", function( ) {
        if (accountSection.classList.contains("hidden")) {
            accountSection.classList.remove("hidden");
            profileSection.classList.add("hidden");
            accountBtn.style.backgroundColor = "#DDDDDD";
            profileBtn.style.backgroundColor = "white";
        } else {
            accountSection.classList.remove("hidden");
        }
    });

    });
   


</script>

<main>  
    <Header />
    <div class="w-10/12 mx-auto">
        <div>
            <div>
                <h1 id="pageType" class="font-bold text-2xl mt-8"> Settings </h1>
                <p> Manage your account settings and preferences </p>
                <hr class="h-px my-8 bg-gray-200 border-0 dark:bg-gray-700">
            </div>
            
        </div>
        <div class="grid grid-cols-5">
            <div>
                <img class="md:hidden" src={hamburger} width="30" height="30" alt="hamburger menu"> 
                <ul class="py-3 hidden md:grid">
                    <button id="profileBtn" class=" w-full rounded-lg text-left text-lg py-2 pl-4"> Profile</button>
                    <button id="accountBtn" class=" w-full rounded-lg text-left text-lg py-2 pl-4"> Account </button>
                    <button id="appearanceBtn" class=" w-full rounded-lg text-left text-lg py-2 pl-4"> Appearance</button>                   
                    <button id="notificationBtn" class=" w-full rounded-lg text-left text-lg py-2 pl-4"> Notifications</button>
                    <button id="paymentoptionsBtn" class=" w-full rounded-lg text-left text-lg py-2 pl-4"> Payment Options </button>                    
                    <button id="displatBtn" class=" w-full rounded-lg text-left text-lg py-2 pl-4"> Display</button>
                </ul>
            </div>
            <div class="col-span-4 w-10/12 ml-3">
                <!-- Profile Section-->
                <div id="profileSection">
                    <div class="my-5">
                        <h1 class="font-bold text-xl"> Profile</h1>
                        <p class="text-sm md:text-md"> This is how others will see you in the site</p>
                        <hr class="h-px my-8 bg-gray-200 border-0 dark:bg-gray-700"> 
                    </div>
                    <div class="my-5">
                        <h1 class="font-bold text-lg"> Username</h1>
                        <input class="pl-2 border rounded-md py-1 mt-2 w-3/4 md:w-80" type="text" placeholder="username"> 
                        <p class="text-black text-opacity-40 text-sm md:text-md"> This is your public display name. It can be your real name or a pseudonym. You can only change this once every 30 days.</p>
                    </div>
                    <div class="my-5">
                        <h1 class="font-bold text-lg"> Email</h1>
                        <input class="pl-2 border rounded-md py-1 mt-2 w-3/4 md:w-80" type="text" placeholder="email"> 
                        <p class="text-black text-opacity-40 text-sm md:text-md "> You can manage verified email addresses in your email settings. </p>
                    </div>
                    <div class="my-5">
                        <h1 class="font-bold text-lg"> Bio </h1>
                        <textarea class="pl-2 border rounded-md py-1 mt-2 w-3/4 md:w-80 resize-none" type="text" placeholder="bio"> </textarea>
                        <p class="text-black text-opacity-40 text-sm md:text-md" > You can @mention other users and organizations to link to them. </p>
                    </div>
                    <div>
                        <button class="p-2 bg-black font-bold text-white text-md rounded-lg"> Update Profile</button>
                    </div>
                </div>
                <!-- Account Section-->
                <div id="accountSection" class="hidden">
                    <div class="my-5">
                        <h1 class="font-bold text-xl"> Account</h1>
                        <p> Update your account settings. Set your preferred language and timezone. </p>
                        <hr class="h-px my-8 bg-gray-200 border-0 dark:bg-gray-700"> 
                    </div>
                    <div>
                        <div class="my-5">
                            <h1 class="font-bold text-lg"> Full Name</h1>
                            <div class="flex-col md:flex-row">
                                <input class="pl-2 border rounded-md mr-2 py-1 mt-2 w-80" type="text" placeholder="First Name"> 
                                <input class="pl-2 border rounded-md py-1 mt-2 w-80" type="text" placeholder="Last Name"> 
                            </div>
                            <p class="text-black text-opacity-40"> Update your name. This will remain private</p>
                        </div>
                    </div>
                    <div class="my-5">
                        <h1 class="font-bold text-lg"> Address</h1>
                        <div class=" flex-col md:flex-row">
                            <input class="pl-2 border rounded-md mr-2 py-1 mt-2 w-6/12" type="text" placeholder="Address"> 
                        </div>
                        <p class="text-black text-opacity-40"> Update your address. This will remain private</p>
                    </div>
                    <button class="p-2 bg-black font-bold text-white text-md rounded-lg"> Update Account</button>
                </div>
               
            </div>
        </div>
       
       
</div>

<Footer />

</main>