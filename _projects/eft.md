---
layout: page
title: On the EFTofLSS
description: Testing the assumptions of the EFTofLSS
# img: assets/img/water_waves.jpg
importance: 1
category: Work
---
<p>An effective theory is an approximate description of a physical system that captures information on relevant scales. To illustrate the idea, consider the problem of describing the motion of water on the surface of an ocean. One approach is to model the water as a fluid, and the surface of the water can be thought of through interacting waves. We call it a large-scale model. Alternatively, one can consider the motion of water as emerging from the interactions of individual water molecules. We call this a small-scale model.
</p>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/water_waves.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/water_molecules.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Alternative descriptions of the same object at different scales. <i>Left</i>: a large-scale model describes the motion of water as interacting waves. <i>Right</i>: a small-scale model describes the motion as emerging from the collective motion of individual molecules.
</div>

<p>Both these models have their advantages and limitations. The large-scale model is accurate on scales large enough so that the individual molecular motions can be ignored, but becomes less accurate as we zoom-in. The small-scale model can accurately model the small scales, but is impractical if we are interested in the large scales, because it gets prohibitively expensive to calculate the individual molecular motions.
</p>

<p>
If we are interested in some intermediate scales, the large-scale model compromises on accuracy and the small-scale model on simplicity. However, it is possible to cleverly combine the two models to treat such scales, which retains the simplicity of the former model, and the accuracy of the latter. This approach falls under the umbrella of an effective theory. 
</p>