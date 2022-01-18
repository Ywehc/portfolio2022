<template>
    <div class="container">
        <canvas id="forest" height="600" width="1200"></canvas>
    </div>
</template>

<script>
import JQuery from 'jquery';
window.$ = JQuery;

// The fantastic function below to procedurally generate the tree was written by Ricky Eckhardt (https://codepen.io/rickyeckhardt/pen/Gkpez) and modified by me.

export default {
    mounted() {
        $(document).ready(function() {
			var canvas = document.getElementById('forest');
			if (canvas.getContext) {
			var ctx = canvas.getContext("2d");
					recursiveTree(ctx, 825, 400, 50, -Math.PI / 2, 13, 13);
				}
			});

        var recursiveTree = function (ctx, startX, startY, length, angle, depth, branchWidth ) {
            var rand = Math.random,
                newLength, newAngle, newDepth, maxBranch = 3,
                endX, endY, maxAngle = 2 * Math.PI / 4,
                subBranches;
            
            ctx.beginPath();
            ctx.moveTo(startX,startY);
            endX = startX + length * Math.cos(angle);
            endY = startY + length * Math.sin(angle);
            ctx.lineCap = 'round';
            ctx.lineWidth = branchWidth;
            ctx.lineTo(endX,endY);
            
            if (depth <= 2) {
                ctx.strokeStyle = "#44a832";
            }
            else {
                ctx.strokeStyle = "black";
            }
            ctx.stroke();
            
            newDepth = depth - 1;
            
            if (!newDepth) {
                return;
            }
            
            subBranches = (rand() * (maxBranch - 1)) + 1;
            
            branchWidth *= 0.7;
            
            for ( var i = 0; i < subBranches; i++ ) {
                newAngle = angle + rand() * maxAngle - maxAngle * 0.5;
                newLength = length * (0.7 + rand() * 0.28);
                recursiveTree(ctx, endX, endY, newLength, newAngle, newDepth, branchWidth);
            }
        };
    }
}
	
</script>

<style lang="scss" scoped>

#forest {
    z-index: 10;
    position: absolute;
    margin-left: -40em;
}

</style>
