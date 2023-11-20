---
layout: post
title: "How I Build D&D Battle Maps in Photoshop"
date: 2023-10-14 04:22:44 -0600
tags: ["d&d", "design", "digital-art"]
excerpt: "Though tools like Dungeondraft are certainly helpful for aspiring game masters, there are moments when one may still want to roll out their own custom built maps in Photoshop."
---

Though tools like [Dungeondraft](https://dungeondraft.net/) are certainly helpful for aspiring game masters, there are moments when one may still want to roll out their own custom built maps in Photoshop. This could be for any number of reasons:

- There may be a desired mood for a scene that requires a more painterly approach to lighting.
- The prebuilt assets in your dungeon building app of choice may not fit a particular dungeon idea that you have.
- You may just need to build a single map to augment a prebuilt campaign module and already own Photoshop.

For myself though, I just prefer a finer degree of control as a personal preference. Below, I outline my approach in how I would put together a basic 5 room dungeon.

## Setup

### Dungeon Dimensions

Before you start building a dungeon, you must first define a few variables for your map. For this tutorial, we'll use the following values.

- **Tile Size in Feet:** 5ft
- **Tile Size in Pixels:** 50px
- **Map Dimensions - Number of Tiles:** 20 X 20
- **Map Dimensions in Pixels:** 1000px X 1000px
- **Wall Thickness in Pixels:** 10px

### Setting up Photoshop

The first thing you need to do is set up Photoshop to allow us to more easily work with gridded maps. Follow these steps:

1. Create a new 1000px X 1000px Photoshop document
2. Navigate to Preferences -> Guides, Grids, & Slices. Set Gridline Every to 50px and Subdivsions to 1. Click Ok.
3. In the top navbar, click on View -> Show and toggle on Grid.
4. In the top navbar, click on View -> Snap To and toggle on Grid.

![Set Grid Lines]({{'/assets/img/posts/dnd-map/dnd-map-1.png' | relative_url }})

This is what you should see after following the previous steps. These grid lines, though visible in Photoshop, will be invisible when the map is eventually exported as an image. These lines are guides to assist us in map building. They can be used to more easily paint walls, region select specific areas of the map, or paint specific tiles with exact precision.

![New Document]({{'/assets/img/posts/dnd-map/dnd-map-2.png' | relative_url }})

### Trace out the Dungeon

Create a new layer and name it "Floor". On that layer, block out the rooms in a solid color. Set the background layer to all black. 

![Floor]({{'/assets/img/posts/dnd-map/dnd-map-3.png' | relative_url }})

Create a new layer and name it "Walls". Pick a new color and select the brush tool. Set the brush size to 10px and the hardness to 100%. Holding down the shift key, outline the dungeon walls along the grid lines with the brush.

![Walls]({{'/assets/img/posts/dnd-map/dnd-map-4.png' | relative_url }})

### Working with Textures

Now that you have a dungeon layout outlined, the next step is to replace these block colors with some detailed textures.

Open the tile image below in Photoshop. Select all, and then click Edit -> Define Pattern in the top navbar. Give the pattern a recognizable name and click Ok.

![Walls]({{'/assets/img/posts/dnd-map/dnd-map-tiles.png' | relative_url }})

![Define Pattern]({{'/assets/img/posts/dnd-map/dnd-map-5.png' | relative_url }})

Go back to your map and double click on the "Floor" layer to open up the Layer Style window. Toggle on Pattern Overlay and select the newly defined pattern from the options.

![Apply Floor Pattern]({{'/assets/img/posts/dnd-map/dnd-map-6.png' | relative_url }})

Repeat the same steps for the "Walls" layer. Feel free to play around with different textures that you think would work best for your dungeon!

![Apply Wall Pattern]({{'/assets/img/posts/dnd-map/dnd-map-7.png' | relative_url }})

The way it is now, the dungeon looks a tad flat. It's hard to distinguish between the walls and floor at first glance. Later on you will paint in more shadow. For a quick base layer to get you started though, open the Layer Style window for the "Walls" layer. Toggle on drop shadow and play around with the values until it looks right to you.

![Add Basic Shadows]({{'/assets/img/posts/dnd-map/dnd-map-8.png' | relative_url }})

### Lighting and Shadow

For a simple game, you could call this map complete. But, you could certainly keep pushing the map further with some custom lighting and shadow.

To better see your map, you may toggle off the display of the grid lines by clicking View -> Show and toggling off Grid in the navbar. You will not need the grid lines much from this point forward.

For starters, I like to apply a simple gradient to the entire image. Create a new layer and call it "Gradient". Make sure this new layer is on top of the previous layers. Select the Gradient tool and choose a subtle set of colors to your liking. I'm going with a set of dark faded blues to simulate a night scene. Starting at the top corner of the image, click and drop to the opposite corner to apply the gradient.

![Apply Gradient]({{'/assets/img/posts/dnd-map/dnd-map-9.png' | relative_url }})

Now set the Blending Mode for the "Gradient" layer to Soft Light.

![Blending Mode Gradient]({{'/assets/img/posts/dnd-map/dnd-map-10.png' | relative_url }})

Next, let's deepen some of these shadows. Create a new layer called "Shadows" and place it between the "Floor" and "Walls" layers. Select the Brush tool and set the Color to black, Hardness to 0%, the Size to 100, and the Opacity to 25%. With the edge of the brush, paint along the walls and corners to deepen the shadow.

![Deepen Shadows]({{'/assets/img/posts/dnd-map/dnd-map-11.png' | relative_url }})

The change is subtle, but the extra shadow makes the scene appear more hostile and unforgiving, giving it a more horrific tone. This same painterly approach to shadow could also be used to elongate shadows for objects placed on the map, like so. Just make sure objects you add to the map are on top of the "Shadow" layer.

![Extend Shadows]({{'/assets/img/posts/dnd-map/dnd-map-12.png' | relative_url }})

For a shadow to be that long though, there should be a significant light source nearby. I'm going to add a fire pit to the scene. To make it cast light, create a new layer above the objects and call it "Light". Next re-enable the grid and region select the room with the light source.

![Set Up Light Source]({{'/assets/img/posts/dnd-map/dnd-map-13.png' | relative_url }})

On the "Light" layer paint in some light using the same technique we used for deepening shadows. Just choose a lighter warm color and a higher opacity.

![Paint the Light]({{'/assets/img/posts/dnd-map/dnd-map-14.png' | relative_url }})

Set the Blending Mode of the "Light" layer to Hard Light. If the lighting looks off, delete some of the lighting and clean it up as you like.

![Paint the Light]({{'/assets/img/posts/dnd-map/dnd-map-15.png' | relative_url }})

### Final Map

This is what the result is when exported as a PNG.

![Paint the Light]({{'/assets/img/posts/dnd-map/dnd-map-final.png' | relative_url }})

While certainly not the most exciting map to play through, it does establish the basic tools and techniques needed to flesh out a more complete map.

- Planning the dimensions of the map
- Outlining the map
- Filling in textures
- Adding objects to the scene
- Applying basic shadows and lighting

While this method certainly takes practice, I've found I can churn maps out far quicker than with tile sets and with a far greater degree of flexibility as well. If I don't like a particular tile texture, I can swap it out without needing to rebuild the entire dungeon. If I need a wall in the middle of a room, I can just paint it there. If I need a map for different times of the day, I can just change the gradient colors.

I hope this has been helpful! Happy map making!
