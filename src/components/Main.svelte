<script>
import Step from "./Step.svelte";

let steps = [
    {
        name: "Programming Language Lexical Analyzer, Parser, and Interpreter",
        icon: "fa-solid fa-computer",
        description:
            "Assemble lexical analyzer with 33 token types, top-down recursive descent parser, and interpreter for programming language with 19 grammar rules in C++.",
    },
    {
        name: "Discord Study Bot",
        icon: "fa-brands fa-discord",
        description:
            "developed a Study Bot that can help you manage your study sessions effectively. With a simple command, it tracks the duration of your study session and provides timely reminders to take breaks every 25 minutes. You also have the flexibility to end your study session whenever you wish..",
    },
    {
        name: "Personal Website",
        icon: "fa-solid fa-globe",
        description:
            "Created my own website with HTML, CSS, JS.",
    },
];

let benefits = [
    {
        metric: "10x",
        name: "a computer science major at NJIT",
        description:"I am a junior student at NJIT with a strong passion for programming and a dedicated team player. I am actively seeking an internship or co-op opportunity in the field of software engineering. My enthusiasm for coding, combined with my commitment to collaborative work, makes me an ideal candidate for any software engineering role."
    },
    {
        name: "a fanatic for making clean and concise code",
        description:"As a computer science major at NJIT, I have honed my abilities to write code that is not only functional but also clean, concise, and highly maintainable. This skill is a cornerstone of effective software development and reflects my commitment to delivering high-quality solutions. Here's how I've cultivated this expertise:"
    },
    {
        name: "an excellent communicator",
        description:
            "Communication is key and it's a paramount value of mine. I believe in transparency and constructive communication above all else. This helps me develop deep relationships and ensures my effectiveness and productivity in any work space with any team.",
    },
];
</script>

<main class = "flex flex-col flex-1 p-4">
    <section id = "introPage" class ="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14">
        <div class = "flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10">
            <h2 class= "font-semibold text-4xl sm:text-5xl md:text-6xl">
                Hi! I'm <span class="poppins text-violet-400">Daniel</span> Lobo <br>Full Stack
                <span class="poppins text-violet-400">Developer</span>
            </h2>
            <p class="text-base sm:text-lg md:text-xl">
                My <span class="text-violet-400">favorite tech</span> includes Python, Java, JavaScript, 
                SvelteKit, Tailwind CSS, C, C++, Bash, Node.js
            </p>
        
            <a href="https://www.linkedin.com/in/csdaniellobo/" class="blueShadow mx-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins 
            relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950 cursor-pointer">
            <div class = "absolute top-0 right-full w-full h-full bg-violet-400 opacity-20
                        group-hover:translate-x-full z-0 duration-200">
            </div>
            <h4 class = "relative z-9">Get in touch &rarr;</h4>
            </a>
        </div>
        <div class="relative shadow-2xl grid place-items-center">
            <img src={"images/pfp.jpg"} alt="Profile image" class= "object-cover z-[2] max-h-[70vh]"/>
        </div>
    </section>
    <section id="projects" class="py-20 lg:py-32 flex flex-col gap-24">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-lg sm:text-xl md:text-2xl">
                A few of my creative endeavors.
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                Curious to <span class= "poppins text-violet-400">see</span> my work?
            </h3>
        </div>
        <a href="https://github.com/DanielLobo2025" target="blank" class = "mx-auto px-4 py-2 rounded-md border border-solid
        border-white flex items-center gap-2 -mb-4 sm:-mb-0-mt-10 hover:border-violet-700 duration-200">
            
        
        <i class="fa-regular fa-circle-play"></i>
            <p>My Github</p>
        </a>
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
            <Step step={steps[0]}>
                <p>
                    Assembled a lexical analyzer with 33 token types, top-down recursive descent parser, 
                    and interpreter for programming language with 19 grammar rules. Created in
                    <strong
                class="text-violet-400"
             >C++</strong>
    
                </p>
            </Step>
            <Step step={steps[1]}>
                <p>developed a Study Bot that can help you manage your study sessions effectively. With a simple command, 
                    it tracks the duration of your study session and provides timely reminders to take breaks every 25 minutes. 
                    You also have the flexibility to end your study session whenever you wish. I recently integrated OpenAi's API to allow users to
                    ask chatgpt study related questions from their own server. Created with 
                     <strong
                        class="text-violet-400">Python and Node.js</strong
                    >.
                </p>
            </Step>
            <Step step={steps[2]}>
                <p>
                    I developed a dynamic and visually appealing web portfolio.This portfolio highlights my technical proficiency but also serves as a 
                    versatile platform for displaying my work and achievements.Created with <strong class="text-violet-400"
                        >SvelteKit & TailwindCSS</strong
                    >.
                 
                </p>
            </Step>
        </div>
    </section>
    <section
        id="about"
        class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative"
    >
        <div
            class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4"
        >
            <h6 class="text-large sm:text-xl md:text-2xl">
                Want to know more?
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                A bit <span class="poppins text-violet-400">about</span> me.
            </h3>
        </div>
        <p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">
            I am . . .
        </p>
        <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
            {#each benefits as benefit, index}
            
                <div class="flex gap-6 sm:gap-8">
                    <p
                        class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold"
                    >
                        0{index + 1}
                    </p>
                    <div class="flex flex-col gap-6 sm:gap-8">
                        <h3 class="text-2xl sm:text-3xl md:text-5xl">
                            {benefit.name}
                        </h3>
                        <p>{benefit.description}</p>
                    </div>
                </div>
            {/each}
        </div>
       
    </section>
</main>