<script lang="ts">
    import Project from "./Project/+page.svelte";
    import Contect from "./Contect/+page.svelte";
    import {Button} from "$lib/components/ui/button";
import {mode} from "mode-watcher";
const lightmodeimage="bcanav.png";
const darkmodeimage="pcana.png";
</script>
<div class="text-3xl font-bold text-center pt-32 py-10">About me</div>
<div class="block flex flex-col pr-5 pl-5 items-center lg:ml-72 sm:flex-row gap-5 ">
    <img src={ $mode === "dark" ? darkmodeimage:lightmodeimage} alt="Mode Based Image" class="h-[320px] w-[320px] items-center rounded-full shadow-primary shadow-[0px_5px_80px_-5px_rgba(0,0,0,3)] mx-7" >

    <h1 class="font-medium w-[250px] text-center mx-7 m-10 ">
        Hello, I am <h class="text-primary">Raghad</h>, a computer science student at um Al-Qura University, and I am interested in web development

        <div class="my-5 ml-7 items-center flex flex-row">
        <Button class="m-2"><a href="#project">project</a></Button>
        <Button class="m-1"><a href="#contect">contect</a></Button>
        </div>

    </h1>

</div>
<div id="project">
    <Project/>
</div>
<div id="contect">
    <Contect/>
</div>