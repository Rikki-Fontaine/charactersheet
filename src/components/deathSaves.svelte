<script lang=ts>
    import { ListBox, ListBoxItem } from '@skeletonlabs/skeleton';
    let success: string[] = [ ];
    let fail: string[] = [ ];
</script>

<div class="flex-col text-center w-1/4">
    <p class="w-3/4 md:w-1/2 ml-10 md:ml-4 underline">Death Saves</p>

    <div class="flex text-center">

        <div class="w-3/4 md:w-1/4 p-2 mt-2 ml-2 text-center rounded-md variant-ghost-secondary">
            <span>Success</span>
            <ListBox multiple>
                <ListBoxItem bind:group={success} name="medium" value="1">1</ListBoxItem>
                <ListBoxItem bind:group={success} name="medium" value="2">2</ListBoxItem>
                <ListBoxItem bind:group={success} name="medium" value="3">3</ListBoxItem>
            </ListBox>
        </div>           

        <div class="w-3/4 md:w-1/4 p-2 mt-2 ml-2 text-center rounded-md variant-ghost-primary">
            <span>Failure</span>
            <ListBox multiple>
                <ListBoxItem bind:group={fail} name="fail" value="1">1</ListBoxItem>
                <ListBoxItem bind:group={fail} name="fail" value="2">2</ListBoxItem>
                <ListBoxItem bind:group={fail} name="fail" value="3">3</ListBoxItem>
            </ListBox>
        </div>           
    </div>
</div>
