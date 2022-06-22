<template>
    <canvas id="c"></canvas>
</template>

<script>
    import { fabric } from 'fabric';
    export default {
        name: 'AppCanvas',
        mounted() {
            var canvas = new fabric.Canvas('c');
            var rectangle = new fabric.Rect({width: 20, height: 20, fill: 'red', left: 10, top: 100, selectable: true});
            canvas.add(rectangle);
        },
    }
</script>