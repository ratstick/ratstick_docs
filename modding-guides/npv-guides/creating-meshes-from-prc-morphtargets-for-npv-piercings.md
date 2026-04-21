---
description: >-
  This will walk you through using the PRC morphtargets to create meshes to use
  PRC piercings on your NPV.
---

# Creating meshes from PRC morphtargets for NPV piercings

## The Theory

Morphtargets are, in essence, just a type of mesh. When you export it, it will show up in Blender just like any other mesh. In game, morphtargets tell the game what shape something should be so that you don't have to make a billion different meshes unique to every single possible shape. It's how we can use all the same meshes for the player head because the morphtargets tell the game how to shape the meshes when a specific option in the character creator is selected.

What we'll be doing, is using the existing piercing meshes and renaming them so we can maintain the material entries, then we'll use the PRC morphtargets to create meshes with the shape we want.

Then, you'll need to run those meshes through the head.blend script so you can shapekey them to your NPV's head.



## Step 1: Preparing the files

### Adding the PRC morphtargets to your project

Since we'll need to run these through the head.blend script, make sure these go in the same folder your other head morphtargets are.

<figure><img src="../../.gitbook/assets/1 (2).png" alt=""><figcaption></figcaption></figure>

After adding the morphtarget, I'm going to rename it so I know which mesh is which.

<figure><img src="../../.gitbook/assets/3 (2).png" alt=""><figcaption></figcaption></figure>

After renaming it, I move it into the morphtargets folder with the rest of the head morphtargets.

Make a copy of one of the existing i1 meshes and name it the exact same way you named the morphtarget.

<figure><img src="../../.gitbook/assets/4 (2).png" alt=""><figcaption></figcaption></figure>

## Step 2: Creating the shaped mesh

Now, export both the morphtarget and the mesh.&#x20;

<figure><img src="../../.gitbook/assets/5 (2).png" alt=""><figcaption></figcaption></figure>

In Blender, import the **morphtarget only**.

<figure><img src="../../.gitbook/assets/6 (1).png" alt=""><figcaption></figcaption></figure>

Make sure it's selected, and then export.

{% hint style="info" %}
That's correct, there is nothing you actually need to do in Blender. We're using the I/O tool to shape the mesh we exported.
{% endhint %}

<figure><img src="../../.gitbook/assets/7 (1).png" alt=""><figcaption></figcaption></figure>

Next, import them back into WolvenKit. You can open up the mesh to double-check the shape.

First, you see we have the material entries we'll need for the piercing textures.

<figure><img src="../../.gitbook/assets/8 (2).png" alt=""><figcaption></figcaption></figure>

You can then switch to the mesh preview tab and see that the mesh now has the same shape as the PRC piercing.

<figure><img src="../../.gitbook/assets/9 (2).png" alt=""><figcaption></figcaption></figure>

All done! Don't forget to shapekey it with the head.blend script!
