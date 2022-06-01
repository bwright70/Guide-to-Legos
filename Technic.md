# Technic

If you want to follow along in the parts studio, here is a link to my [original document](https://cvilleschools.onshape.com/documents/18c55e9aeb64057e8e0fbb6a/w/5c06b8e3c4dcf6e948152fa4/e/18df3578f02c775cfcadaef9?configuration=List_8xTqWDMkkCG2Mw%3D_2x2%3BList_ArQ6GsCPNSkQoQ%3DDefault%3BList_Izy0ldJ6UfParG%3DDefault%3BList_tmPjPdZ9wrB2lD%3DDefault&renderMode=0&uiState=6290d24be366b652b2773d0f). Navigate to the technic folder and open the technic pins part studio. You might have to navigate to all tabs first because I'm pretty sure the link puts you into the square bricks folder. 

## Lets Begin

Right off the bat I have a confession to make. 

I only ever got Technic pins working one way. This tutorial will teach you how to make technic pins and other similar things, and more importantly how to make bricks that are cross compatible with actual lego technic peices. But this is a warning. 

#### THE TECHNIC PINS NEED TO BE CHANGED SLIGHTLY TO WORK WITH REAL LEGOS!

## Ok with that out of the way lets actually begin. 

Here is what I'm talking about when I say [Technic Pin](https://www.bricklink.com/v2/catalog/catalogitem.page?P=2780#T=C)

Begin by sketching a center point circle on the origin and dimensioning it 5mm + #Unit (6.5mm)

Extrude add it #Half_Unit

Then sketch a second center point circle on your disk and dimension it 5mm. 

Extrude it up (8 * #Rows)mm - #Half_Unit or 7.25mm. 

<img src="Photos/Technic.PNG">

I highly recommend using the variable equations because if you end up changing #Unit in the future your parts studios will update with you. I also find it helpful to understand how I arrived at a number after the fact. 

In this case I relized that the Technic Pins would best be designed around a mirror and that each length of half of the pin needed to be equal to 8mm because they end up perfectly connecting two [1x2 Technic Bricks](https://www.bricklink.com/v2/catalog/catalogitem.page?P=3700#T=C). 

This means that the total length of a technic pin is 16mm because that is the width of a 1x2 brick. 

Anyway tangent aside lets get back to the part. 

Sketch another center circle on the new extrusion and dimension it equal to #Rod_Width

#### (Rod_Width also requires futher testing and it's just a place holder)

Extrude remove the sketch up to the bottom of the 6.5mm circle

<img src="Photos/Technic(1).PNG">

Next create yet another centerpoint circle on the top of the pillar and dimension it so thats its 0.25mm larger than the circle. Then extrude only the outside ring #Half_Unit/2 or 0.375mm 

This creates a small lip that allows the technic pin to stay secure. 

<img src="Photos/Technic(2).PNG">

Now we're going to make the part of the technic pin that doesn't work. 

Create a Sketch on the lip of the Technic Pin. 

Draw a horizontal construction line from the center of the circle to the edge. Then draw two horizontal lines on the lip of the pin symmetric around the center line and #Half_Unit away from each other. 

<img src="Photos/Technic(3).PNG">

Extrude remove the new sketch a very specific number: #Unit * 2 + #Half_Unit * 1.33 or 3.998mm 

Just trust me on this one cause I don't remember why I chose this to be the distance but I'm like 85% sure it's pretty close to correct. 

Finally mirror the extrude remove over whatever plane works to make it show up on the other side of the lip. For me it was the right plane

<img src="Photos/Technic(4).PNG">  

