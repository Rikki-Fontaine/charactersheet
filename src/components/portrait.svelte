<script lang>
    import {Avatar} from '@skeletonlabs/skeleton';
    let src = "/goat.jpg";
    let name = "Sam";
    let playerClass = "Bard";
    let level = 10;
    let race = "Satyr";
    let background = "Traveler";
    let experience = 1000;
</script>

<!--This needs a slightly better layout-->

<div class="flex justify-center md:justify-around mb-2 p-2 text-sm md:text-base">
    <div class="grid grid-cols-1 gap-5 mt-2 text-left">
        <span>Name: {name}</span>
        <span>Class: {playerClass}</span>
        <span>Background: {background}</span>
    </div>

    <Avatar src={src} width="w-32" rounded="rounded-full" />

    <div class="grid grid-cols-1 mt-2 gap-5 text-right">
        <span>Level: {level}</span>
        <span>Race: {race}</span>
        <span>Experience: {experience}</span>
    </div>
</div>
<hr>