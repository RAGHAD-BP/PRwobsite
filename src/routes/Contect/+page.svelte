<script lang="ts">
    import { Input } from "$lib/components/ui/input/index.js";
    import { Label } from "$lib/components/ui/label/index.js";
    import {Textarea} from "$lib/components/ui/textarea/index.js";
    import {Button} from "$lib/components/ui/button";
</script>
<div class="text-3xl font-bold text-center pt-32 py-10 ">Let's Talk!</div>
<form class="m-5 p-8 bg-secondary">
    <div class="grid w-full items-center gap-3"><div class="flex flex-row  gap-3"><div>
        <Label for="name">Name</Label>
        <Input required  name="name" id="name" placeholder="write your name" /></div><div>
        <Label for="email">Email</Label>
        <Input required type="email" name="email" id="email" placeholder="example1@gmail.com"/></div></div>
        <div>
            <Label for="subject">Subject</Label>
            <Input required name="subject" id="subject" placeholder="....."/></div>
    <div>
        <Label for="massege">Massege</Label>
        <Textarea required name="massege" id="massege" placeholder="write your massge" />
            </div>
        <Button type="submit">Send</Button>
    </div>
</form>