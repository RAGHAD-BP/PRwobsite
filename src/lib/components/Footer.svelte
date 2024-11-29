<script lang="ts">
import Button from "$lib/components/ui/button/button.svelte";
</script>

<div class="flex justify-between items-baseline  w-[100dvw] bg-secondary text-secondary-foreground py-4 px-4 ">
    <span class="font-light ">
    © {new Date().getFullYear()} by Raghad Alsouwayhi <span/>
    </span>
    <div class=" flex justify-between gap-4">
    <span class="flex flex-col items-center">
        <span class="font-semibold">Email</span>
        <a href="mailto:raghad11ali88@gmail.com">raghad11ali88@gmail.com</a>
    </span>
        <span class="flex flex-col items-center">
            <span class="font-semibold">Foolow</span>
            <div class="flex flex-row">

    <Button variant="ghost" size="icon" href="https://www.linkedin.com/in/raghad-alsuwayhi-976b38307?trk=contact-info">
        <svg
                class="h-auto w-6"
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 24 24"
        ><path
                fill="currentColor"
                d="M6.94 5a2 2 0 1 1-4-.002a2 2 0 0 1 4 .002M7 8.48H3V21h4zm6.32 0H9.34V21h3.94v-6.57c0-3.66 4.77-4 4.77 0V21H22v-7.93c0-6.17-7.06-5.94-8.72-2.91z"
        /></svg
        >
    </Button>
            </div>
        </span>
        </div>
</div>