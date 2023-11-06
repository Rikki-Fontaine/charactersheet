<script lang="ts">
let stats=[
{stat : "STR", value: 10, bonus: 0},
{stat : "DEX", value: 16, bonus: 3},
{stat : "CON", value: 12, bonus: 1},
{stat : "WIS", value: 14, bonus: 2},
{stat : "INT", value: 9, bonus: -1},
{stat : "CHA", value: 18, bonus: 4}
]


</script>


<div class="snap-x scroll-px-4 snap-mandatory scroll-smooth flex gap-4 overflow-x-auto px-2 py-5">
	{#each stats as {stat, value, bonus}, i}
		<div class="snap-start shrink-0 card py-20 w-40 md:w-80 text-center variant-ghost-primary">
            <span>{stat} : {value}</span>
            <hr class="mt-1">
            {#if bonus > 0}
            <span class="badge variant-filled-success mt-3">{#if bonus >= 0}+{/if}{bonus}</span> <!--If it's a negative bonus variant should be filled error-->
            {:else}
            <span class="badge variant-filled-error mt-3">{#if bonus >= 0}+{/if}{bonus}</span>
            {/if}
        </div>
	{/each}
</div>
