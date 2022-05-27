# Slant

If you want to follow along in the parts studio, here is a link to my [original document](https://cvilleschools.onshape.com/documents/18c55e9aeb64057e8e0fbb6a/w/5c06b8e3c4dcf6e948152fa4/e/18df3578f02c775cfcadaef9?configuration=List_8xTqWDMkkCG2Mw%3D_2x2%3BList_ArQ6GsCPNSkQoQ%3DDefault%3BList_Izy0ldJ6UfParG%3DDefault%3BList_tmPjPdZ9wrB2lD%3DDefault&renderMode=0&uiState=6290d24be366b652b2773d0f). Navigate to the Square Bricks folder and find the Part Studio called Slant. 

### Lets Begin

To start make a copy of your original parts studio with the bricks. You can make this in your original parts studio as well, but the more you do this, the more convoluted your part studio is and the assemblies get laggier. 

Making slants is actually very simple. I would recomend designing this on the 2x3 or 1x3 brick. If you are following along in the parts studio ignore Slant Corners. I had those working at one point, but they're broken and I don't feel like fixing them. You can go through and see what I did, but I don't intend to make them work again. 

First make a sketch on the front face of your brick. Like So:
<img src="Photos/Slants.PNG">

Next draw a verticle construction line connecting the top and bottom of your part and dimension it 8mm away from the left edge

Then draw two lines. One starts at the top of the conntruction line and ends at the right edge. Dimension it so that its #Unit away from the bottom right corner. The second begins at the bottom Right corner and is parrallel to the first. 
<img src="Photos/Slants(1).PNG">

(If you're following along in the parts studio you'll notice that I have two sketches and one of them is really weird. Ignore it.)

Next draw a corner rectangle whose bottom two corners are the top of the construction line and the top right corner. Dimension it's height to be any number greater than #Stud_Height. 

Extrude Remove (up to face of the opposite side) the rectangle and the triangle made by the top parrallel line. 
<img src="Photos/Slants(2).PNG">

Finally extrude add (up to face of the opposite side) the parrallelagram created by the two parrallel lines. 
<img src="Photos/Slants(3).PNG">

And there you go now you have a slant that works on any configurations. 

# Inverse Slants

If you are following along in document navigate to the Inverse Slants parts studio.

### Lets Begin Again

I would once again recommend making a copy of the original parts studio. You can also delete the bottom cylinder and Tube features because they're never used in this part.

First make a Sketch on the bottom face of the brick and draw a Rectangle with it's left side 5mm from the left edge and the rest of the sides coincident with the brick. 

<img src="Photos/Slants(4).PNG">

Extrude Add the Rectangle up to the inside of the brick. 

Next sketch on the front face of your brick. Draw a line from the bottom edge to the right edge. The lines bottom point should be 8mm away from the left edge and #Unit away from the top edge. 

<img src="Photos/Slants(5).PNG">

Extrude remove (up to face of the opposite side) the bottom triangle created by the new sketch. 
