<script>
    import {icons} from '../icons';

    export let type = 'proiUi';
    export let color;
    export let scale = 20;
</script>
{#if icons[type]}
    <svg id="icon" data-name="{icons[type].name}" viewBox="0 0 12 12" style="width: {scale}px; height: {scale}px;">
        <title>{icons[type].name}-icon</title>
        <g id="icon-content" data-name="content">
            {#each icons[type].paths as path}
                <path d="{path}" style="fill:{color ? color : icons[type].color}"/>
            {/each}
        </g>
    </svg>
{:else}
    {(console.error(`incorrect type: ${type}`))}
{/if}
