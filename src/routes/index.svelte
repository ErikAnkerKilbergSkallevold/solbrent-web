<script>

import { loop_guard } from "svelte/internal";

</script>

<!DOCTYPE html>
<html lang="en">
    <header>
        <meta name="viewport" content="width=device-width,
        initial-scale = 1.0">
        <meta http-equiv="X-UA-Compatible" content="ie=edge" />
        <meta charset="UTF-8">
        <title>Solbrent</title>
        
    </header>    
    <body>
        

        <div class="flex fixed top-0 left-0 h-screen w-16 flex-col bg-gray-900 text-white shadow-lg">
            <img class="relative flex items-center justify-center h-12 w-12 mt-2 mb-2 mx-auto shadow-lg" src="static\assets\applogo.png" alt="todo">
        
            <div class="sidebar-icon group group">
                <a href="https://github.com/ErikAnkerKilbergSkallevold">
                    <img class="sidebar-icon" src="static\assets\images\gitMe.png" alt="Github Logo with my face">
                </a>
                <div class="sidebar-icon-tooltip group-hover:scale-100">
                    <p>My GitHub!</p>
                </div>
            </div>
        
            <div class="sidebar-icon group group">
                <a href="https://github.com/ErikAnkerKilbergSkallevold/Solbrent">
                    <img class="sidebar-icon" src="static\assets\images\gitApp.png" alt="Github Logo with the app logo">
                </a>
                <div class="sidebar-icon-tooltip group-hover:scale-100">
                    <p>The apps GitHub!</p>
                </div>
            </div>
            
            <div class="sidebar-icon group group">
                <a href="https://github.com/ErikAnkerKilbergSkallevold/solbrent-web">
                    <img class="sidebar-icon" src="static\assets\images\gitWeb.png" alt="Github Logo with the internet logo">
                </a>
                <div class="sidebar-icon-tooltip group-hover:scale-100">
                    <p>This webpages GitHub!</p>
                </div>
            </div>
            
            <div class="sidebar-icon group group">
                <a href="static\assets\downloads\solbrent.apk" download="Solbrent.apk" title="Download Solbrent Link">
                    <img class="sidebar-icon" src="static\assets\images\download_icon.svg" alt="Download button">
                </a>
                <div class="sidebar-icon-tooltip group-hover:scale-100">
                    <p>Download app!</p>
                </div>
            </div>
        </div>

        <div class="intro max-w-full ml-6 -z-10">
            <h1 class="text-center font-thin md:text-9xl ml-6 text-7xl text-gray-900">Solbrent</h1>
            <!-- svelte-ignore a11y-media-has-caption -->
            <video src="static\assets\Video\SolbrentWebVideo_AME\appIntro_FHD_16-9.mp4"></video>
        </div>      

        <section class="mt-12">
            <div class="container reveal">
                <h1 class="text-3xl text-gray-900 text-center pt-0 ml-12 mt-0">Aldri bli <strong class="bg-gradient-to-l">solbrent</strong> igjen</h1>
            </div>
        </section>

        <section class="mt-24">
            <div class="container reveal">
                <h1 class="text-3xl text-gray-900 text-center pt-0 ml-12 mt-0">Last ned <strong class="bg-gradient-to-l">solbrent</strong> og få kontroll på solen</h1>
            </div>
        </section>

        <!-- Popup 1 -->
        <div>    
            <div class="bg-white bg-opacity-100">
                <section class="mt-24 wrapper ml-12">
                    <div class="container reveal">
                        <div class="sm:w-1/3 sm:mt-24 sm:left lg:left">
                            <img class="top-12 md:max-w-full justify-center ml-12 md:mx-auto mb-0 bottom-0" src="static\assets\images\phones\homePhone.png" alt="Home page shown on a phone screen">
                        </div>
                        <div class="right mt-12 ml-12 mr-6 sm:m-0 sm:p-0 md:mx-auto md:mt-8 lg:mt-36 max-w-fit md:max-w-full bg-white rounded-xl shadow-md overflow-hidden">
                            <div class="md:flex">
                            <div class="md:shrink-0">
                                <img class="h-44 w-44 m-auto object-cover md:h-full md:w-fit" src="static\assets\images\eyes.png" alt="Eye emoji">
                            </div>
                            <div class="lg:p-8 md:p-2 sm:p-0 w-screen max-w-fit">
                                <div class="uppercase tracking-wide text-sm text-yellow-500 font-semibold">All in one</div>
                                <p class="block mt-1 text-lg leading-tight font-medium text-black">Get all the relevant information at a glance</p>
                                <p class="mt-2 text-slate-500">Don't waste time going through multiple menues and pages. Noone wants to stare at a weather app when they're out having fun. Get all the information you need at a glance.</p>
                            </div>
                            </div>
                        </div>
                    </div>
                </section>
            </div>
        </div>


        <!-- Popup 2 -->
        <div>    
            <div class="bg-white bg-opacity-100">
                <section class="mt-24 wrapper ml-12">
                    <div class="container reveal">
                        <div class="sm:w-1/3 sm:mt-24 sm:left lg:left">
                            <img class="top-12 md:max-w-full justify-center ml-6 md:mx-auto mb-0 bottom-0" src="static\assets\images\phones\detaljPhone.png" alt="Home page shown on a phone screen">
                        </div>
                        <div class="right mt-12 ml-12 mr-6 sm:m-0 sm:p-0 md:mx-auto md:mt-8 lg:mt-36 max-w-fit md:max-w-full bg-white rounded-xl shadow-md overflow-hidden">
                            <div class="md:flex">
                            <div class="md:shrink-0">
                                <img class="h-44 w-44 m-auto object-cover md:h-full md:w-fit" src="static\assets\images\nerd.png" alt="Nerd emoji">
                            </div>
                            <div class="lg:p-8 md:p-2 sm:p-0 w-screen max-w-fit">
                                <div class="uppercase tracking-wide text-sm text-yellow-500 font-semibold">Detailed</div>
                                <p class="block mt-1 text-lg leading-tight font-medium text-black">Go for a dive (if you want)</p>
                                <p class="mt-2 text-slate-500">Want a 24-hour forecast? Tips to avoid sunburn? Get a scale for how much uvi there is? Swipe up on the homescreen and get additional info about the sun.</p>
                            </div>
                            </div>
                        </div>
                    </div>
                </section>
            </div>
        </div> 

        <!-- Popup 3 -->
        <div>    
            <div class="bg-white bg-opacity-100">
                <section class="mt-24 wrapper ml-12">
                    <div class="container reveal">
                        <div class="sm:w-1/3 sm:mt-12 sm:left lg:left">
                            <img class="top-12 md:max-w-full justify-center ml-6 md:mx-auto mb-0 bottom-0" src="static\assets\images\phones\skinTone.png" alt="Home page shown on a phone screen">
                        </div>
                        <div class="right mt-12 ml-12 mr-6 sm:m-0 sm:p-0 md:mx-auto md:mt-8 lg:mt-36 max-w-fit md:max-w-full bg-white rounded-xl shadow-md overflow-hidden">
                            <div class="md:flex">
                            <div class="md:shrink-0">
                                <img class="h-44 w-44 m-auto object-cover md:h-full md:w-fit" src="static\assets\images\hudfargebilde.png" alt="Skin color emojies">
                            </div>
                            <div class="lg:p-8 md:p-2 sm:p-0 w-screen max-w-fit">
                                <div class="uppercase tracking-wide text-sm text-yellow-500 font-semibold">Made for you</div>
                                <p class="block mt-1 text-lg leading-tight font-medium text-black">Reacts to your skintype</p>
                                <p class="mt-2 text-slate-500">Different skin types react differently to the sun. Pick your skintype from the Fitzpatrick scale and see how the app reacts.</p>
                            </div>
                            </div>
                        </div>
                    </div>
                </section>
            </div>
        </div> 

        <!-- Popup 4 -->
        <div>    
            <div class="bg-white bg-opacity-100">
                <section class="mt-24 wrapper ml-12">
                    <div class="container reveal">
                        <div class="sm:w-1/3 sm:left lg:left">
                            <img class="top-12 md:max-w-full justify-center ml-12 md:mx-auto mb-0 bottom-0" src="static\assets\images\phones\timerPhone.png" alt="Home page shown on a phone screen">
                        </div>
                        <div class="right mt-12 ml-12 mr-6 sm:m-0 sm:p-0 md:mx-auto md:mt-8 lg:mt-36 max-w-fit md:max-w-full bg-white rounded-xl shadow-md overflow-hidden">
                            <div class="md:flex">
                            <div class="md:shrink-0">
                                <img class="h-44 w-44 m-auto object-cover md:h-full md:w-fit" src="static\assets\images\clock.png" alt="Clock emoji">
                            </div>
                            <div class="lg:p-8 md:p-2 sm:p-0 w-screen max-w-fit">
                                <div class="uppercase tracking-wide text-sm text-yellow-500 font-semibold">Countdown</div>
                                <p class="block mt-1 text-lg leading-tight font-medium text-black">3...2...1...</p>
                                <p class="mt-2 text-slate-500">...Apply more sunscreen. Get notified by the app when it's time for more sunscreen. And if you do get burnt it will also give you some advice on what to do.</p>
                            </div>
                            </div>
                        </div>
                    </div>
                </section>
            </div>
        </div>

        <!-- Download -->
        <div>    
            <div class="gradient lg:ml-48 lg:mb-0 lg:m-24 ml-24 mr-12 bg-opacity-100 rounded-3xl shadow-2xl">
                <section class="mt-24 wrapper ml-12">
                    <div class="container reveal">
                        <div class="sm:w-1/3 sm:left lg:left">
                            <img class="top-12 md:max-w-full justify-center -ml-6 md:mx-auto mb-0 bottom-0" src="static\assets\applogo.png" alt="Home page shown on a phone screen">
                        </div>
                        <div class="right mt-12 mr-12 mx-auto my-auto sm:m-0 sm:p-0 md:mx-auto md:mt-8 lg:mt-12 lg:mr-12 max-w-fit md:max-w-full bg-green-400 rounded-xl shadow-md overflow-hidden">
                            <div class="md:flex">
                            <div class="md:shrink-0">
                                <a href="static\assets\downloads\solbrent.apk" download="Solbrent.apk" title="Download Solbrent Link">
                                    <img class="h-44 w-44 object-cover md:h-full md:w-fit bg-white hover:bg-black transition-all ease-in hover:cursor-pointer" src="static\assets\images\android.png" alt="Clickable Android logo download button">
                                </a>
                            </div>
                            <div class="lg:p-8 md:p-2 sm:p-0 w-screen max-w-fit">
                                <div class="uppercase tracking-wide text-sm text-white font-semibold">Download</div>
                                <p class="block mt-1 text-lg leading-tight font-medium text-black">Want to try it out?</p>
                                <p class="mt-2 text-slate-500">By downloading, I here by understand that this app was created as student project and that some information might be wrong. I also understand that there might be security holes and that the app is currently available in Norwegian. No warranty is provided.</p>
                            </div>
                            </div>
                        </div>
                    </div>
                </section>
            </div>
        </div>
        
        <footer class="text-center">
            <a href="https://github.com/ErikAnkerKilbergSkallevold/solbrent-web" class="text-gray-900 hover:underline hover:text-blue-600">Made by me!</a>
            <br>
            <a href="https://www.freepik.com/free-vector/vector-smartphone-with-blank-white-screen_7588609.htm#&position=8&from_view=author" class="text-gray-900 hover:underline hover:text-blue-600">Phone template provided by upklyak</a>
        </footer>
        
    <script>
        function reveal() {
        var reveals = document.querySelectorAll(".reveal");

        for (var i = 0; i < reveals.length; i++) {
            var windowHeight = window.innerHeight;
            var elementTop = reveals[i].getBoundingClientRect().top;
            var elementVisible = 150;

            if (elementTop < windowHeight - elementVisible) {
            reveals[i].classList.add("active");
            } else {
            reveals[i].classList.remove("active");
            }
        }
        }

        window.addEventListener("scroll", reveal);
    </script>

    <script>
        const intro = document.querySelector(".intro");
        const video = intro.querySelector("video");
        const text = intro.querySelector("h1");
        //END SECTION
        const section = document.querySelector("section");
        const end = section.querySelector("h1");

        //SCROLLMAGIC
        const controller = new ScrollMagic.Controller();

        //Scenes
        let scene = new ScrollMagic.Scene({
        duration: 6000,
        triggerElement: intro,
        triggerHook: 0
        })
        .setPin(intro)
        .addTo(controller);

        //Text Animation
        const textAnim = TweenMax.fromTo(text, 3, { opacity: 1 }, { opacity: 0 });

        let scene2 = new ScrollMagic.Scene({
        duration: 1000,
        triggerElement: intro,
        triggerHook: 0
        })
        .setTween(textAnim)
        .addTo(controller);

        //Video Animation
        let accelamount = 0.1;
        let scrollpos = 0;
        let delay = 0;

        scene.on("update", e => {
        scrollpos = e.scrollPos / 1000;
        });

        setInterval(() => {
        delay += (scrollpos - delay) * accelamount;

        video.currentTime = delay;
        }, 33.3);
    </script>
</html>



<svelte:head>
        <script
        src="https://cdnjs.cloudflare.com/ajax/libs/ScrollMagic/2.0.7/ScrollMagic.min.js"
        integrity="sha256-2p2tRZlPowp3P/04Pw2rqVCSbhyV/IB7ZEVUglrDS/c="
        crossorigin="anonymous"
    ></script>
    <script
        src="https://cdnjs.cloudflare.com/ajax/libs/ScrollMagic/2.0.7/plugins/animation.gsap.js"
        integrity="sha256-peenofh8a9TIqKdPKIeQE7mJvuwh+J0To7nslvpj1jI="
        crossorigin="anonymous"
    ></script>
    <script
        src="https://cdnjs.cloudflare.com/ajax/libs/ScrollMagic/2.0.7/plugins/debug.addIndicators.js"
        integrity="sha256-31FC/OT6XpfjAhj9FuXjw5/wPXXawCAjJQ29E23/XPk="
        crossorigin="anonymous"
    ></script>
    <script
        src="https://cdnjs.cloudflare.com/ajax/libs/gsap/2.1.3/TweenMax.min.js"
        integrity="sha256-lPE3wjN2a7ABWHbGz7+MKBJaykyzqCbU96BJWjio86U="
        crossorigin="anonymous"
    ></script>
</svelte:head>