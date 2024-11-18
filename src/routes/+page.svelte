<script lang="ts">
    import Project from "./Project/+page.svelte";
    import Contact from "./Contect/+page.svelte";
    import {Button} from "$lib/components/ui/button";
</script>
<div>--------About me----------</div>
<div class="block pr-5 pl-5  flex justify-items-end justify-center ">
<div class="shadow-xl  flex flex-col  w-[320px] mr-5 h-fit">
    <img src="/bcanav.png " class="h-[320px] w-[320px]" >
    <div class="font-bold items-center">Raghad Alsuwayhi</div>
    <div>programmer</div>
    <div class="bg-card h-[30px]">
        jjjh</div>
</div>
    <div class="font-medium w-[250px] text-center ">
        Hello i'm Raghad a student in
        umm alqra universite my migor is
        compouter sciens and i a web delovbor
        and programmer
        <div class="m-5">
        <Button>project</Button>
        <Button>contect</Button>
        </div>
    </div>

</div>

<div>
<Project/>
</div>
<div>
<Contact/>
</div>