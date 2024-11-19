<script lang="ts">
    import Project from "./Project/+page.svelte";
    import Contact from "./Contect/+page.svelte";
    import {Button} from "$lib/components/ui/button";
</script>
<div>--------About me----------</div>
<div class="block pr-5 pl-5  flex justify-items-end justify-center m-5 sm:items-start">
    <img src="/bcanav.png " class="h-[320px] w-[320px] rounded-full shadow-primary shadow-[0_10px_80px_-15px_rgba(0,0,0,3)] mx-7" >

    <h1 class="font-medium w-[250px] text-center mx-7">
        Hello i'm Raghad a student in
        umm alqra universite my migor is
        compouter sciens and i a web delovbor
        and programmer

        <div class="my-5  items-center ">
        <Button>project</Button>
        <Button>contect</Button>
        </div>

    </h1>

</div>


<div>
<Project/>
</div>
<div>
<Contact/>
</div>