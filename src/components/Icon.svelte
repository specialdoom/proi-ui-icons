<script>
    import {icons} from '../icons';

    export let type = 'error';
    export let color;

    let clr = color ? color : icons[type].color;
</script>

<style>
    .sd-icon{
        height: 20px;
        width: 20px;
    }
</style>

<div class="sd-icon" style="fill: {clr}">
    <svg id="icon" data-name="{icons[type].name}" viewBox="0 0 12 12">
        <title>{icons[type].name}-icon</title>
        <g id="icon-content" data-name="content">
            <path d="{icons[type].path}"/>
        </g>
    </svg>
</div>
