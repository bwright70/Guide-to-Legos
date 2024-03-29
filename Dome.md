# Dome 

If you want to follow along in the parts studio, here is a link to my [original document](https://cvilleschools.onshape.com/documents/18c55e9aeb64057e8e0fbb6a/w/5c06b8e3c4dcf6e948152fa4/e/18df3578f02c775cfcadaef9?configuration=List_8xTqWDMkkCG2Mw%3D_2x2%3BList_ArQ6GsCPNSkQoQ%3DDefault%3BList_Izy0ldJ6UfParG%3DDefault%3BList_tmPjPdZ9wrB2lD%3DDefault&renderMode=0&uiState=6290d24be366b652b2773d0f). Navigate to the Other folder and open the Weird Dome part studio. The link puts you into the square bricks folder so youre going to want to go to home first. 

## Lets Begin 

You're going to want to make a new parts studio for this one because it's ver different from your normal brick. 

I debated whether or not I should include this one because its not a very common brick and doesn't share much with any other bricks, but I think it's probably important to learn just because of how weird it is. 

Also I'm just doing a tutorial on the 2x2 Dome for two reasons: 
1. I don't think the 4x4 is really necessary to learn 
2. I may or may not have accidently broken the 4x4 making this tutorial and I don't feel like fixing it

### Dome 

This is the [Brick](https://www.bricklink.com/v2/catalog/catalogitem.page?P=553b#T=C) we're talking about

#### Disclaimer: This part is a bunch of nonsense numbers. Making legos is a bunch of trial and error because there are no offical dimensions for legos. Don't ask how I got the numbers I did because I really don't remember. 

First make a sketch on the front plane. Make a corner rectangle from the origin and delete the top line. 

Dimension the verticle lines to be #Height(9.7mm) - #Unit(1.5mm). I'll explain why later. 

Dimension the horizontal line to be #Length(8mm)

Now make a new top line but don't just connect it to the right side line. Instead dimension it to be (5mm + (#Unit/2))/2. Just copy the equation and drop it into onshape. 

Now make a conic arc from the bottom right corner to the end of the top line. Attach it's little arc point to the top of the right line and dimension the arc to be 0.45.

<img src="Photos/Dome(1).PNG">

Revolve the sketch around the origin mate connector. (If you're following along with the document you'll notice I have an extra sketch and did a sweep instead of a revolve. I honestly have no idea why I choose to do that but a revolve is easier) 

Now select the bottom face and select hollow. Set the Shell thickness to #Unit(1.5mm) 

<img src="Photos/Dome(2).PNG">

Now make a sketch on the bottom face of the dome and make a circle dimensioned to 16mm. Extrude the whole circle #Unit(1.5mm). This extrude should fully cover the opening you just made which I know seems counter-intuitive, but it's necessary for the creating the tube later. 

Now flip your part over and make a sketch on the top of the dome. Make two circles centered on the top of the dome: one dimensioned to be #Rod_Thickness(3.2mm) and the other dimensioned to be #Tube_Width(5mm). Then extrude out the space between the two #Stud_Height(1.8mm). 

Boom. You gotta a Stud. You can also throw on a 0.25mm fillet to the outside edge of the stud to make it look nicer and make assembly easier. 

<img src="Photos/Dome(3).PNG">

Alright now I'm going to show you a little trick thats necessary to make this part work. 

Right click the bottom face of the dome and create a section view.

<img src="Photos/Dome(4).PNG">

Click on the arrow and drag it up into the part. Leave the top half the the part visible. You'll notice that we are now able to select thing inside the part. 

Select top of the inside of the dome and make a sketch. 

<img src="Photos/Dome(5).PNG">

You can turn off the section view now by clicking on the little cube in the top right below the camera orientation cube. "Turn section view off" is at the bottom. 

In your new sketch you're going to make the Axel sketch used in the [Technic](Technic.md) and [Circles](Circles.md) tutorials. 

Make a circle centered on the origin and dimensioned to be #Tube_Width(5mm). 

Next make a horizontal and verticle construction line passing through the origin. 

Now make the axel shape, and dimension the lines to be ((#Half_Unit/2) + #Unit) away from each other. 

<img src="Photos/Dome(7).PNG">

Extrude everything outside the cross down (#Height - #Unit - 2mm), so that an axel  could fit into the gap 

Now make a sketch on the bottom of the dome. Create a centerpoint circle on the origin and dimension it #Unit(1.5mm) away from the outer edge of the dome. 

Create 4 lines tangent to the circle: 2 horizontal and 2 verticle. This is very similar sketch to the one in the [Circles](Circles.md) tutorial. 

Extrude remove the center of the circle and the curved trapezoid looking areas #Unit(1.5mm). 

<img src="Photos/Dome(8).PNG">

Next make a sketch on a section of the bottom of the Dome that's left

Create a circle centered on the origin dimensioned to be #Tube_Width(5mm). 

Ok now select Loft. The settings should be Surface and New. The Profiles should be the circle created in the inverted axel sketch and the circle you just created. 

Now create a Thicken (It's right next to loft). The settings should look like this: 

<img src="Photos/Dome(9).PNG">

You'll notice the loft created a surface underneath in the same section as new parts. This is what you select to thicken. Once your thicken is complete just hide the surface. 

Add a 0.25mm fillet to the inverted axels and then you're done! 

<img src="Photos/Dome(10).PNG">

## Reflection 

### Dome 

So the Domes comes in three sections: 

1. The stud on the top
2. The dome section 
3. The stud connection points 

The reason that the dome is dimensioned to a height of #Height(9.7mm) - #Unit(1.5mm) is because otherwise the dome would be an extra #Unit(1.5mm) tall. For most bricks the main section of the brick and a connector points are one and the same with a total height of #Height(9.7mm), but with the dome those are two seperate features because it's very hard to work with curves in onshape. 

I was initially confused as to why I had made the bottom connector points soild. Turns out I did have a reason because it breaks if I change it. In simple terms it was necessary because the central tube is a loft and you need two faces to select for a loft. It's weird and dumb and took me several attempts but it works; which is the best way to summerize most of my projects. 

