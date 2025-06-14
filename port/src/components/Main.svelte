<script>
    import Step from './Step.svelte';

    let steps = [
        {name: 'Professional Skills', icon: 'fa-solid fa-burger'},
        {name: 'Cleaning and Organisation', icon: 'fa-solid fa-soap'},
        {name: 'Creative Skills', icon: 'fa-solid fa-palette'},
        {name: 'Soft Skills', icon: 'fa-solid fa-brain'},
        {name: 'Bonus Talents', icon: 'fa-solid fa-star'},
    ]

    let benefits = [
        {name: "Employee of the month", description: "Over 374 consecutive months"},
        {name: " Saved the Krusty Krab", description: "multiple times from Plankton’s evil plots"},
        {name: "Winner of Jellyfish Fields Fishing Tournament", description: "Able to catch even rare jellyfish like the Queen Jellyfish"},
        {name: "Perfect Health Inspection Score", description: "for Krusty Krab"},
        {name: "Broadway musical (within canon)", description: "starred in it."},

    ]
</script>

<main class="flex flex-col flex-1 p-4">
    <section id="introPage" class="bg-cover grid grid-cols-1 lg:grid grid-cols-2 gap-10 py-8 sm:py-14">
        <div class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10">
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
                Hi! I am <span class="text-yellow-300">Spongebob</span> Squarepants<br/>
            Your beloved <span class="text-yellow-300">animated </span> character.</h2>

            <p >The endlessly optimistic <span class="text-yellow-300"> sea sponge</span> who lives in a pineapple under the sea. 
                Whether you're a longtime fan or just diving in, explore the characters, 
                iconic episodes, and quirky humor that have made SpongeBob a global sensation 
                for over two decades. Grab a Krabby Patty and join us on a jellyfishing adventure!</p>

            <a href="#contacts" target="_blank"
            class="mx-auto lg:mr-auto text-base sm:text-lg md:text-xl poppins relative
            overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950">
                <div 
                    class="absolute top-0 right-full w-full h-full bg-yellow-400 opacity-40
                    group-hover:translate-x-full z-0 duration-200">
                    <h4 class="relative z-9">Get in touch &rarr;</h4>
                </div>
            </a>
        </div>
        <div class="relative  grid place-items-center">
            <img src={'images/spongebob.png'} alt="" class="object-cover z-[2] max-h-[70vh]">
        </div>
 
    </section>

    <section id="projects" class="py-20 lg:py-32 flex flex-col gap-24">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-lg sm:text-xl md:text-2xl">
                A few of my creative skills.
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                🧽 SpongeBob SquarePants – <span class="text-yellow-300">Skills & Abilities</span>
            </h3>
        </div>
        <a href="https://www.youtube.com/watch?v=-CF4MXpDyNs&t=15s" target="_blank" 
                class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 
                sm:-mb-0 -mt-10 hover:border-yellow-400 duration-200">
                <i class="fa-regular fa-circle-play"></i>
                <p class="text-yellow-300">Watch the video</p>
        </a>
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
            <Step step={steps[0]}>
                <p>
                    <strong class="text-yellow-300"> Cook Level Legendary</strong>  – Expert grill master at the Krusty Krab. Known for perfect Krabby Patties.<br/>
                    <strong class="text-yellow-300">Fast Food Multitasking</strong> – Can take orders, cook, serve, and clean simultaneously with precision.<br/>
                    <strong class="text-yellow-300">Bubble Artistry</strong> – Master of bubble-blowing; capable of creating complex bubble shapes and scenes.<br/>
                    <strong class="text-yellow-300">Certified in Jellyfishing </strong>– Experienced in the art of jellyfish catching, with fast reflexes and patience.<br/>
                    <strong class="text-yellow-300">Customer Service Enthusiast </strong>– Overly enthusiastic; always eager to please customers (even when they’re annoyed).<br/>
                </p>
            </Step>
            <Step step={steps[1]}>
                <p>
                    <strong class="text-yellow-300">Spotless Sanitation</strong> – Passionate about cleanliness. Known to scrub homes, workplaces, and public spaces to perfection.
                    <strong class="text-yellow-300">Hyper-Organized </strong>– Keeps workspaces tidy and utensils polished.
                </p>
            </Step>
            <Step step={steps[2]}>
                <p>
                    <strong class="text-yellow-300">Undersea Sculptor</strong> – Built a detailed replica of the Krusty Krab using sand.
                    <strong class="text-yellow-300">Imaginative Thinking </strong>– "IMAGINATION" is his favorite tool. Great for brainstorming and storytelling.
                    <strong class="text-yellow-300">Karate Chopping</strong> – Performs martial arts (karate) with SpongeBob-style flair—frequently with Sandy Cheeks.
                </p>
            </Step>
            <Step step={steps[3]}>
                <p>
                    <strong class="text-yellow-300">Optimism & Enthusiasm </strong>– Maintains a positive attitude no matter the situation.
                    <strong class="text-yellow-300">Team Player</strong> – Works well with others, even when they’re grumpy (Squidward).
                    <strong class="text-yellow-300">Resilience</strong> – Keeps going even when he fails (like boating school).
                </p>
            </Step>
            <Step step={steps[4]}>
                <p>
                    <strong class="text-yellow-300">Snail Whisperer </strong>– Understands and cares deeply for his pet snail, Gary.
                    <strong class="text-yellow-300">Musician</strong> – Plays various instruments (including his nose, ukulele, and jellyfish jelly-based tunes).
                    <strong class="text-yellow-300">Multilingual </strong>– Fluent in "Dolphin Censor Beeps" (occasionally).
                </p>
            </Step>
        </div>
    </section>

    <section id="about" class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative">
        <div class="flex flex-col gap-2 text-center relative 
                    before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-yellow-300 
                    after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-yellow-300 py-4">
            <h6 class="text-large sm:text-xl md:text-2xl ">Want to know more?</h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                A bit <span class="savate text-yellow-300">about</span> me
            </h3>
        </div>

        <p class="mx-auto savate font-semibold text-lg sm:text-xl md:text-2xl">I have achieved...</p>
        <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
            {#each benefits as benefit, index}
            <div class="flex gap-6 sm:gap-8">
                <p class="savate text-4xl sm:text-5xl md:text-6xl text-sky-600 font-semibold">
                    0{index + 1}
                </p>
                <div class="flex flex-col gap-6 sm:gap-8">
                    <h3 class="text-2xl sm:text-3xl md:text-5xl ">{benefit.name}</h3>
                    <p class="text-yellow-300">{benefit.description}</p>
                </div>
            </div>
            {/each}
        </div>

        <h5 class="text-2xl sm:text-3xl font-semibold text-center savate">
            The <span class="text-yellow-300 ">Complete</span> Package</h5>
        <div class="flex flex-col overflow-x-scroll gap-10 max-w-[800px] mx-auto w-full">
            <table class="bg-white text-slate-700 rounded text-center">
                <thead class="border-b border-solid border-slate-200">
                    <tr class="">
                        <th/>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #1</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #2</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #3</th>
                        <th class="whitespace-nowrap bg-yellow-300 text-white p-4 px-8">Me!</th>
                    </tr>
                </thead>
                <tbody>
                    <tr class="border-b border-solid border-slate-200">
                        <td class="border-b border-solid border-white pl-4 pr-8 py-4 font-semibold
                        text-sm whitespace-nowrap">Dedication</td>
                        <td><i class="fa-solid fa-xmark text-red-500"></i></td>
                        <td><i class="fa-solid fa-check text-green-500"></i></td>
                        <td><i class="fa-solid fa-xmark text-red-500"></i></td>
                        <td><i class="fa-solid fa-check text-green-500"></i></td>
                    </tr>
                    <tr class="border-b border-solid border-slate-200">
                        <td class="border-b border-solid border-white pl-4 pr-8 py-4 font-semibold
                        text-sm whitespace-nowrap">Critical Thought</td>
                        <td><i class="fa-solid fa-check text-green-500"></i></td>
                        <td><i class="fa-solid fa-xmark text-red-500"></i></td>
                        <td><i class="fa-solid fa-xmark text-red-500"></i></td>
                        <td><i class="fa-solid fa-check text-green-500"></i></td>
                    </tr>
                    <tr class="border-b border-solid border-slate-200">
                        <td class="border-b border-solid border-white pl-4 pr-8 py-4 font-semibold
                        text-sm whitespace-nowrap">Interpersonal Skills</td>
                        <td><i class="fa-solid fa-xmark text-red-500"></i></td>
                        <td><i class="fa-solid fa-check text-green-500"></i></td>
                        <td><i class="fa-solid fa-check text-green-500"></i></td>
                        <td><i class="fa-solid fa-check text-green-500"></i></td>
                    </tr>
                    <tr class="border-b border-solid border-slate-200">
                        <td class="border-b border-solid border-white pl-4 pr-8 py-4 font-semibold
                        text-sm whitespace-nowrap">Awesomeness!</td>
                        <td><i class="fa-solid fa-xmark text-red-500"></i></td>
                        <td><i class="fa-solid fa-xmark text-red-500"></i></td>
                        <td><i class="fa-solid fa-xmark text-red-500"></i></td>
                        <td><i class="fa-solid fa-check text-green-500"></i></td>
                    </tr>
                </tbody>
            </table>
        </div>

        <div class="mx-auto -mt-12 italic sm:hidden opacity-50">
            <p>Scroll to see more &rAarr;</p>
        </div>
        <p class="mx-auto">So why not hang out with me?</p>
    </section>
</main>