<script lang="ts">
    import Project from "./Project/+page.svelte";
    import Contect from "./Contect/+page.svelte";
    import {Button} from "$lib/components/ui/button";
import {mode} from "mode-watcher";
const lightmodeimage="raghad_alsuwayhi.png";
const darkmodeimage="raghad_alsuwayhi.png";
</script>
<div class="text-3xl font-bold text-center pt-32 py-10">About me</div>
<div class="block flex flex-col pr-5 pl-5 items-center lg:ml-72 sm:flex-row gap-5 ">
    <img src={ $mode === "dark" ? darkmodeimage:lightmodeimage} alt="Mode Based Image" class="h-[320px] w-[320px] items-center rounded-full shadow-primary shadow-[0px_1px_20px_-10px] mx-7" >

    <h1 class="font-medium w-[250px] text-center mx-7 m-10 ">
        Hello, I am <span class="text-primary font-bold" >Raghad Alsuwayhi</span> A programmer, I am interested in web development 

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
