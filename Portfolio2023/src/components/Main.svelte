<script>
    import Step from "./Step.svelte";

    let steps = [
        {name: "Axel Store", icons: "fa-solid fa-cart-shopping", description: "Axel Store est un magazin"},
        {name: "Ultimate Todos", icons: "fa-solid fa-list-check", description: "Todo list"},
        {name: "Pokedex", icons: "fa-solid fa-diagram-project", description: "Un pokedex en ligne"},
    ];
</script>

<main class="flex flex-col flex-1 p-4">
    <section id="introPage" class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14">
        <div class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10">
            <h2 class= "font-semibold text-4xl sm:text-5xl md:text-6xl">
                Bonjour ! Je suis <span class="poppins text-violet-400">Axel</span> Siepak <br/> Full Stack <span class="poppins text-violet-400">Developer</span>
            </h2>
            <p class="text-base sm:text-lg md;text-xl">
                My <span class="poppins text-violet-400">favorite tech</span> include Javascript 
                (NEXT.JS or Sveltkit), TailwindCSS, Node.js +Express.js & PostgreSQL or Firebase/Firestore!
            </p>
            <button class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950">
                <div class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200" />
                <h4 class="relative z-9">Get in touch &rarr;</h4>
            </button>
        </div>
        <div class="relative shadow-2xl grid place-items-center">
            <img src={"images/profile.png"} alt="my face" class="object-cover z-[2] max-h-[70vh]" />
        </div>
    </section>
    <section class="py-20 lg:py-32 flex flex-col gap-24" id="projects">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-large sm:text-xl md:text-2xl">
            A few of my creatives endeavors.
            </h6>
            <h3 class="font-emibold text-3xl sm:text5xl">
                Curious to <span class poppins text-violet-400>see</span> my work?
            </h3>    
        </div>
        <a href="https://www.youtube.com/watch?v=dQw4w9WgXcQ"
            target="_blank"
            class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0-mt-10 hover:border-violet-700 duration-200">
            <i class="fa-regular fa-circle-play"></i>
            <p>Watch the video</p>
            </a>
            <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
                <Step step={steps[0]}>
                
                </Step>
                <Step step={steps[1]}>
                
                </Step>
                <Step step={steps[2]}>
                
                </Step>
            </div>
    </section>
</main>