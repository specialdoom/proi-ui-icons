<script>
    import {icons} from '../icons';

    export let type = 'proiUi';
    export let scale = 20;
</script>

<style>
    .sd-icon {
        height: 20px;
        width: 20px;
    }
</style>

<div class="sd-icon" style="height: {scale}px; width: {scale}px;">
    <svg id="icon" data-name="{icons[type].name}" viewBox="0 0 12 12">
        <title>{icons[type].name}-icon</title>
        <g id="icon-content" data-name="content">
            <path d="{icons[type].path}" style="{icons[type].style ? icons[type].style+';' : ''}{icons[type].hasStroke ? 'stroke:': 'fill:'}{icons[type].color}"/>
        </g>
    </svg>
</div>
