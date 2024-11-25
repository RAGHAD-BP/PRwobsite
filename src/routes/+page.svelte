<script lang="ts">
    import Project from "./Project/+page.svelte";
    import Contact from "./Contect/+page.svelte";
    import {Button} from "$lib/components/ui/button";
</script>
<div class="text-3xl font-bold text-center">Rusme</div>

<div class="block flex flex-col pr-5 pl-5 m-10 items-center lg:ml-72 sm:flex-row  ">
    <img src="/bcanav.png " class="h-[320px] w-[320px] items-center rounded-full shadow-primary shadow-[0px_5px_80px_-5px_rgba(0,0,0,3)] mx-7" >

    <h1 class="font-medium w-[250px] text-center mx-7 m-10 ">
        Hello i'm Raghad a student in
        umm alqra universite my migor is
        compouter sciens and i a web delovbor
        and programmer

        <div class="my-5 ml-7 items-center flex flex-row">
        <Button class="m-2">project</Button>
        <Button class="m-1">contect</Button>
        </div>

    </h1>

</div>


<div>
<Project/>
</div>
<div>
<Contact/>
</div>