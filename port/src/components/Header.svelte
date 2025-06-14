<script>
	//import { Link } from "react-router-dom";

    export let y;

    let tabs = [
        { name: "Projects", link: "#projects"},
        { name: "About me", link: "#about"}

    ]
</script>

<header class={"sticky z-[10] top-0 duration-200 px-6 flex items-center justify-between border border-solid " + (
    y > 0 ? "py-4 bg-sky-800 border-violet-950" : "py-6 bg-transparent border-transparent"
)}>
    <h1 class="font-medium ">
        <b class="text-yellow-400 font-bold Savate">Spongebob</b> Squarepants
    </h1>
    <div class="sm:flex items-center gap-4 hidden">
        {#each tabs as tab, index}
            <a class="duration-200 hover:text-yellow-400" href={tab.link}>
                <p>{tab.name}</p>
            </a>
        {/each}
    </div>
    <a href="#" target="_blank"
        class="blue-shadow relative overflow-hidden px-5 py-2 group rounded-full bg-white text-slate-950"    
    >
        <div 
            class="absolute top-0 right-full w-full h-full bg-yellow-400 opacity-20
            group-hover:translate-x-full z-0 duration-200
        ">
            <h4 class="relative z-9">Get in touch</h4>
        </div>
    </a>
</header>