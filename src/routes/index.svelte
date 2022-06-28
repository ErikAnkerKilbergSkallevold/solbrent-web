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
            <img class="relative flex items-center justify-center h-12 w-12 mt-2 mb-2 mx-auto shadow-lg" src="src\assets\applogo.png" alt="todo">
        
            <div class="sidebar-icon group group">
                <img class="sidebar-icon" src="src\assets\icons\ac_plug-0.png" alt="todo">
                <div class="sidebar-icon-tooltip group-hover:scale-100">
                    <p>Tooltip!</p>
                </div>
            </div>
        
            <div class="sidebar-icon group group">
                <img class="sidebar-icon" src="src\assets\icons\calendar-0.png" alt="todo">
                <div class="sidebar-icon-tooltip group-hover:scale-100">
                    <p>Tooltip!</p>
                </div>
            </div>
            
            <div class="sidebar-icon group group">
                <img class="sidebar-icon" src="src\assets\icons\battery.png" alt="todo">
                <div class="sidebar-icon-tooltip group-hover:scale-100">
                    <p>Tooltip!</p>
                </div>
            </div>
            
            <div class="sidebar-icon group group">
                <img class="sidebar-icon" src="src\assets\icons\briefcase-0.png" alt="todo">
                <div class="sidebar-icon-tooltip group-hover:scale-100">
                    <p>Tooltip!</p>
                </div>
            </div>
        </div>

        <div class="intro -z-10">
            <h1 class="text-center font-thin text-9xl text-gray-900">Solbrent</h1>
            <!-- svelte-ignore a11y-media-has-caption -->
            <video src="src\assets\Video\SolbrentWebVideo_AME\appIntro_FHD_16-9.mp4"></video>
        </div>      

        <section class="mt-12">
            <div class="container reveal">
                <h1 class="text-3xl text-gray-900 text-center font-bold pt-0 ml-12 mt-0">Aldri bli <strong class="bg-gradient-to-l">solbrent</strong> igjen</h1>
            </div>
        </section>

        <section class="mt-24">
            <div class="container reveal">
                <h1 class="text-3xl text-gray-900 text-center font-bold pt-0 ml-12 mt-0">Last ned <strong class="bg-gradient-to-l">solbrent</strong> og få kontroll på solen</h1>
            </div>
        </section>

    
        <div class="bg-indigo-100">    
            <div class="bg-white bg-opacity-100">
                <section class="mt-24">
                    <div class="container reveal">
                        <div class="max-w-md mx-auto bg-white rounded-xl shadow-md overflow-hidden md:max-w-2xl">
                            <div class="md:flex">
                            <div class="md:shrink-0">
                                <img class="h-48 w-full object-cover md:h-full md:w-48" src="src\assets\Screenshots\Kveld.png" alt="Man looking at item at a store">
                            </div>
                            <div class="p-8">
                                <div class="uppercase tracking-wide text-sm text-indigo-500 font-semibold">Case study</div>
                                <a href="#" class="block mt-1 text-lg leading-tight font-medium text-black hover:underline">Finding customers for your new business</a>
                                <p class="mt-2 text-slate-500">Getting a new business off the ground is a lot of hard work. Here are five ideas you can use to find your first customers.</p>
                            </div>
                            </div>
                        </div>
                    </div>
                </section>
            </div>
        </div>

        <div class="bg-yellow-600">
            <div class="bg-green-900 bg-opacity-100">
                <section class="mt-24">
                    <div class="container reveal">
                        <div class="max-w-md mx-auto bg-white rounded-xl shadow-md overflow-hidden md:max-w-2xl">
                            <div class="md:flex">
                            <div class="md:shrink-0">
                                <img class="h-48 w-full object-cover md:h-full md:w-48" src="src\assets\Screenshots\Kveld.png" alt="Man looking at item at a store">
                            </div>
                            <div class="p-8">
                                <div class="uppercase tracking-wide text-sm text-indigo-500 font-semibold">Case study</div>
                                <a href="#" class="block mt-1 text-lg leading-tight font-medium text-black hover:underline">Finding customers for your new business</a>
                                <p class="mt-2 text-slate-500">Getting a new business off the ground is a lot of hard work. Here are five ideas you can use to find your first customers.</p>
                            </div>
                            </div>
                        </div>
                    </div>
                </section>
            </div>
        </div>
    </body>  


    
    <footer class="flex fixed bottom-0 mx-auto w-screen h-16 justify-center">
        <p class="font-medium  text-center">Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
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
        .addIndicators()
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
        console.log(scrollpos, delay);

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