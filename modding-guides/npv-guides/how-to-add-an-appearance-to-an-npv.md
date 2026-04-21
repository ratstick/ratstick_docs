---
description: >-
  This will walk you through how to duplicate an appearance to create new
  appearance in your NPV .app file.
---

# How to add an appearance to an NPV

Commissioned an NPV or had someone make one for you and want to add new appearances yourself? It’s easy! Well, sort of. All the hard work has been done, but there are still some things you’ll want to consider. Here’s a guide walking you through it, step by step.

### Disclaimer

I love subfolders and organizing my NPVs. The screenshots I’ll be sharing are from a mostly vanilla fem V NPV that I was commissioned to make. You’ll see my stupidly detailed folder organization for clothing meshes and textures. If you want to use this in your own projects, you can [download it here](https://drive.google.com/file/d/1McSM228BlsY-4HRoe-lGqPQUGybtkBpT/view?usp=sharing)!

These steps will be the same for adding new hairstyles, tattoos, cyberware, to a new appearance and not the base appearance.

### The Mr. Potato Head and Barbie Dress-Up Metaphor

The .app file tells the game what to load when spawning the character entity.

The .ent file tells the game what file to reference for a given entity to load its appearances.

The .app file is where most of the work takes place. It’s where we’ll start. You can think of it like a Mr. Potato Head doll. The components are the eyes, nose, ears, mouth, hats, bowtie of the Mr. Potato Head doll. When we add items to the .app file, we’re playing dress up with our Mr. Potato Head or Barbie.

It’s not the player, so certain scripts and mechanics don’t apply to it. That means we don’t need a lot of frameworks like More Head Meshes or More Body Meshes. You want to add additional cyberware? You can just add the mesh!

You may still need files from certain texture frameworks, but you’ll find that out when you’re beginning to custom path textures.

### What does “custom pathing” mean, and why do we do it?

Custom pathing is changing the folder structure or the name of a file so that vanilla or other modded files don’t overwrite what you’re putting together. This means that if I have Arkhe’s Universal Skin Tone mod installed, but your NPV uses a different skin file, then your file wouldn’t be overwritten by me having that mod installed.

I take a broad approach to custom pathing and path nearly everything that isn’t an engine file or file type not commonly edited. I still recommend doing this for vanilla clothing items, as replacers are still used for some clothing items. In general, I recommend custom pathing the following file types:

* .mesh
* .mi
* .xbm
* .mlsetup
* .mlmask

## Adding new appearances

#### Step 1: The project

If you haven’t done it already, and if the mod maker didn’t send you the project, go ahead and make your own project now.

Open WolvenKit and select “create a new project”. Fill out the stuff. Make sure you use underscores instead of spaces. WolvenKit will freak out, and your shit may not work if you use spaces in folders and such.

[(full size image)](https://drive.google.com/file/d/1QJ0QRXlIhAszugR6qcsRjUTFO6uxc-I-/view?usp=drive_link)

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXc53L4dqcUvLVBIKjNqILv66VpP2UGcHBRW-R0cpgRo96gUfE_1IcfzggHuIZcn7ZEufCQIX7fHMrU2I9iNLKxnFeJHz3HIQ_TrE7RYTPenUzOFvliAFgyOoTelqDZnVQ62DAkGEw?key=v-1XJeip1aB1Hl1kfJwyYA" alt=""><figcaption></figcaption></figure>

#### Step 2: Duplicating an existing appearance

Since all the hard work has been done for you with the base appearance, you can duplicate an existing appearance. Personally, I usually duplicate one with the same t0 submeshes hidden because I frequently forget to unhide them. (We’ll get to this in a later step).

Find your .app file and click the blue button to open it (you’ll see it when you hover the file).

[(full size image)](https://drive.google.com/file/d/1rqZfhSiJiAUUnHJWlNMj5eh-CptHlXvd/view?usp=drive_link)

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdD3Pym03emaTjazBn2TiQQxZtHTUSNxyvIBAyoMYiNUmUDixGib9dJ7KmXUz6Wzw3fi_uzEmx_SAXYSyXLNkU6JNDfoBSE5__PRfcp-NpOYnY62tQvnOPbp135LVa9Nsq1TjMPJA?key=v-1XJeip1aB1Hl1kfJwyYA" alt=""><figcaption></figcaption></figure>

Right-click on the appearance you want to duplicate and select “Duplicate in Array/Buffer”.

[(full size image)](https://drive.google.com/file/d/1n2rOAqXSH9FhHud5sWOVsiSImaf7e4IH/view?usp=drive_link)

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfJH_-7ALScaKvWJgvmHrzLCt19GZjkFwKogIdYc7jUTUy_jcGqLLty69OTDZjcono0_PXJ3oEzRJl3POYxldD2oJ8hO_F19Zp3FoKZ1H6wpFxYnLoVEZxiSOk1Lgnx7lqap1DEeA?key=v-1XJeip1aB1Hl1kfJwyYA" alt=""><figcaption></figcaption></figure>

It is IMPERATIVE that you change the name of the appearance. No appearance can have the same name. After duplicating, make sure the new appearance is selected. In the right pane, you’ll see a field that says “name”, that’s where you can change the appearance name. Remember!! You must use underscores, no spaces!

[(full size image)](https://drive.google.com/file/d/1ENCKZdPk0UKU567KG5mz8NSFSdUDQDx1/view?usp=drive_link)

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeebgYQs7ny8h-667xGiuLRho8pPM60BCVY2XsR1yV53SHcYCLqTZlPsgqjmkiznsSlnNyf12pr0tvFhaiK8xqCRPoJmBcaoMA2yYEzQw48ZB-EkWn5fXrLXXD3gj5wRhLqZ15VIQ?key=v-1XJeip1aB1Hl1kfJwyYA" alt=""><figcaption></figcaption></figure>

\
Step 3: Playing Barbie Dress-Up (Adding items)

Once the name has been changed, click the carat next to the appearance to expand it, then click the carat next to “components”.  Scroll down to find the clothing components. Your .app file may look different. Modded items will usually have their own mesh names. For vanilla items, you can find the items that start with the following:

* t1 (inner torso)
* t2 (outer torso)
* s1 (shoes)
* h1 and h2 (headwear)
* l1 (legs)
* g1 (gloves)
* i1 (items, e.g., pouches and bags)

In some template .app files, clothing has its own section.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcIdinpLeTe7vNealGhAMxTzjp_-TwP4KI8qlyZJAwVpu87NdLS_65hU2vkYnWOu8IJujO_xrj0cHIpdCGQvb71P9ImUKCmkewWHMnp2kdvR3iGY6_HsncJ4EEyIJgzYWyvRHWp?key=v-1XJeip1aB1Hl1kfJwyYA" alt=""><figcaption></figcaption></figure>

I don’t want the sunglasses in this appearance, so I’m going to delete it. Right-click on the item and select “Delete Item in Array/Buffer”.

[(full size image)](https://drive.google.com/file/d/1lcSfzW_4zA62j9LB5JMZT_qvl0ffAkPV/view?usp=drive_link)

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXf3rbp98qJ-56Y2QpZsPvf3XDE7zp7GW6tfV2pSyGHUZ4Yv7vMzL3SLt6tzB8bEaZTFNaQBEvG_dtPwshg2NQO4cKVe_-r1AHHsQw_E4HP8YTGegW0PD9CShAeqJbahX-giV_NNbQ?key=v-1XJeip1aB1Hl1kfJwyYA" alt=""><figcaption></figcaption></figure>

Now we can get to playing Barbie dress-up! I want to change the shoes. You can either search for the name of the item if you know what it is, or go through the asset browser. You can toggle on the mod browser to find modded items.

[(full size image)](https://drive.google.com/file/d/1JNgZXHyUt2-_zoylhi0jsBw_CYwPd8a-/view?usp=drive_link)

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXd3Wi65stCF1t8EaL9Wa6gMIC23eSEuW9YTSEsTjBqz9nW67vU23h6Zz4yOUB1VBIP56Te7RdXUUISBFMdaA14B0oZ0d7z-KxnKHmKtutZyEtMS8ki4E8cb-XfGBXbI6zSCwqx0QA?key=v-1XJeip1aB1Hl1kfJwyYA" alt=""><figcaption></figcaption></figure>

I want to use the converse. Right-click on the .mesh (pma = player male average / ma = male average; pwa = player woman average / wa = woman average) and click “Add selected items to the project”. This will duplicate the folder structure in your project as well.

Remember, we generally want to custom path most items.&#x20;

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdTPMKZY-X5AiZkroz4YiOBK1IMjGtulIKo2PPFN_uXm8b70YWTQmqZzZITiMZrqFFzNhNnrA_uWz03ops1g6sK4fb6Td2FhGHmYlYBqCKMonO0vjKa4RW1IBCWdh27luyWGSF1Yw?key=v-1XJeip1aB1Hl1kfJwyYA" alt=""><figcaption></figcaption></figure>

I’m going to add a new subfolder (right click on one of the folders) to “feet” for the converse and add another subfolder inside that for the textures. You can also rename the mesh, however I prefer a more organized file structure as I find it easier to navigate, especially if I ever need to change textures!

Drag and drop the .mesh into the new subfolder.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXckqukG0_Czl4dZDzc_kqs7iZcUjYiPXqCFnUHmVA-UOVH7V3gnssYkG0IDUIqA0aVTXw6Fm9Z3WLH_qOGkytGdo1F7DMYROb1SJAB7gnPBJ4OkAUQqs0b9evV7VgZspFiCGCau9w?key=v-1XJeip1aB1Hl1kfJwyYA" alt=""><figcaption></figcaption></figure>

I’m going to swap the existing boot component in the .app file for the converse. You’ll want to change the name, the path to the .mesh, and enter the mesh appearance you want to use.

Right-click on the mesh and select “copy relative path to game file”.&#x20;

[(full size image)](https://drive.google.com/file/d/16NwdbaoQJUftO6jbk1C1SkhDn3DDLH8i/view?usp=drive_link)

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcJu53aurmj8arFgrdF0KzZ8RE_Ns33UbALrWxbvSPPc9Ukd4XACFsmhmE7wBye5yrM5qqD2McUHsAUgPdrEFzng68v6YcWHFqUxpgdsJUkq-3MPCWgthrfTYiezjzBeqYhTxpAqg?key=v-1XJeip1aB1Hl1kfJwyYA" alt=""><figcaption></figcaption></figure>

Then paste it into the “DepotPath” section on the right pane. The component can be renamed to whatever you want. I’m going to put “converse”.

[(full size image)](https://drive.google.com/file/d/18uPaPyhm0N0wewQTJLAbIcJZUGzPxNvC/view?usp=drive_link)

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXd4LQNANRHFYtYWwwMtebAKEOa0M00kvzVzMVW8nPD4gbssdlUXfvqhI8Qu4PHXhQhq6jKctYAhgKi_UsgGFpR66MMY6lSMarr_kD8RFi0asJq9H06Lj55YYvLMSbWOW5CaHU46WQ?key=v-1XJeip1aB1Hl1kfJwyYA" alt=""><figcaption></figcaption></figure>

Now we need to find the mesh appearance and clean up any unused mesh appearances. This just keeps it nice and tidy and easy to find the materials you actually need to change. Just like we did when opening the .app file, hover over the mesh and click the blue button to open it.

The first section you see contains the mesh appearance names, and these are what we’ll put in the meshAppearance field. I like the look of the black converse, so I’m going to choose the “black” meshAppearance.

[(full size image)](https://drive.google.com/file/d/1BcTmoPgo3o8ccKqUxhXMKOciOTZ_RHR5/view?usp=drive_link)

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXctekJHMAeUaIAaKUl5UXyW2APawliR6AND4fZIZA6lTvD4LK69UmyAIvwH25HQJsoXzHdBa-OdCh2E2wxb05yoQh3hWB7QvjxNaO9Q-7JoA0SnyaM-6bLwOAXcjGvlyJovMYa-?key=v-1XJeip1aB1Hl1kfJwyYA" alt=""><figcaption></figcaption></figure>

The component in the .app should now have the mesh appearance, component name, and path to the mesh changed.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdam4xnsBczhEpSlYUiVYVIBBfD1CXHT2h_iiWRlGcESVbxVRf-we2o699bUnzwbqbzK_-Jbbro8m-jr9C-sQ_xt6uagd1PLBCQbaOxNirvV6myYp4rTHmpMucbudOtLPrQfsGjFw?key=v-1XJeip1aB1Hl1kfJwyYA" alt=""><figcaption></figcaption></figure>

Now, it’s time to clean up the mesh appearances! If you use more than one appearance in the mesh, it’s fine to keep those entries in the mesh file. I only want to use the black appearance, so I’m going to delete the rest of the material entries. WolvenKit has a very handy tool that will do this part for you. First, select the appearance entries you don’t want, then right click and hit “Delete Item in Array/Buffer”.

[(full size image)](https://drive.google.com/file/d/1f3eKiKU2BueJR-D1VmgdoegDOkJox5Bl/view?usp=drive_link)

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfGD7zlTwFb1DhqxbDNWkMktGbBGvq571lNAF7Fv865BdGqo0_Kljn8AKZlMlm5xFcesxxCGQd6yexu-ye5HeZ3YXhqeUbZ7GQn8HneYihQPGpl6817lKregN22uMkqUZU9hKWr?key=v-1XJeip1aB1Hl1kfJwyYA" alt=""><figcaption></figcaption></figure>

Now, we can use a function in WolvenKit to clean up the entries we don’t need in the localMaterialBuffer and materialEntries. Click on “Clean up” and then “Delete unused materials”.\
[(full size image)](https://drive.google.com/file/d/1rg2x4flQF2Pvve0fqzeT8x3YV-JLufua/view?usp=drive_link)

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXe0uoPuR09eq2EDJECWtbIsZINJ45-cVh91c_zsCg8YoQEScezO6wO4-3u0S5xwC_OvGHhhKmy-RtYh4BRrzAu2GCau-KKlIdm4ueRXbC2uTVhl7f4HNfEOh40JuzLn3vDQzz8vvA?key=v-1XJeip1aB1Hl1kfJwyYA" alt=""><figcaption></figcaption></figure>

Everyone say “thank you WolvenKit devs.”

Now to edit the path of the textures. Find the localMaterialBuffer and click the carat on the left to expand it. Do the same thing for materials, CMaterialInstance and the values. These contain the paths to the textures we’re going to change.

[(full size image)](https://drive.google.com/file/d/1QOG1HXxYe9bX0rRnPKufplSMVfrNBTuY/view?usp=drive_link)

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdU0JpOtLxcNDnHh1BAv7mK8WQANcsIbF3cp42YN1C2U6vLN-TQ9IHSAmbLO6S7jaOh-nT4VZhdgZ7COwhLize_ZyBYUw9sqFGB8wcz9FKRcfZ-Zrkn1fUBPHrt4_-HDbB1Vkp3Dw?key=v-1XJeip1aB1Hl1kfJwyYA" alt=""><figcaption></figcaption></figure>

Click the yellow arrow to add the texture to your project. We can ignore the baseMaterial because that’s an engine\materials file and I don’t think those are ever changed in any mod.

Just like when we added the mesh to our project, the textures will replicate the folder structure.&#x20;

[(full size image)](https://drive.google.com/file/d/1i-3PEtRQAovcbwcYQ5E--jq0UQZcqJc2/view?usp=drive_link)

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeaMeq0xYVOuvfDtjM5WsqYKfp9w0LIaZdfAJ0UNsra8YeNxY6IAZsYLK4vF-3y14WRU0YmtosauoisgY3dGdL2M3oPM4q2_pNNd06y9MjlDvW6dxQna-1vl01mVUl6Y3z63ykW?key=v-1XJeip1aB1Hl1kfJwyYA" alt=""><figcaption></figcaption></figure>

And just like we did with the mesh, we want to drag and drop those into the “textures” subfolder.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXd6hNFGda3fCA78j2cWDRSvyLB1F52lrPY9Q2vWzdBDq5WNfR9-8vdELNSFrIlcr1pw82Raaoyjlw0uAT9NBZQPO4-fQVPWxC5vE-iBfuKW74PjAWYzds0yE22xTmoHdMPhMgLz?key=v-1XJeip1aB1Hl1kfJwyYA" alt=""><figcaption></figcaption></figure>

Just like we did the mesh path, right-click on the texture, select “copy relative path” and paste it into the corresponding field in the .mesh. Then save it. Do this for all the textures that need to be pathed.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXd1qWoTbtMstxomzVjWlCXYPP1AwSGOaSUVbEBOJz-7s0lVNeN5T5uu805fZMlkaR_xN_NG4DHC_t2f9wGYfbhTHAIVFTzsR8stx8nZ3bAyok8NTztK94wuyy-Vfax17wgp6VShsA?key=v-1XJeip1aB1Hl1kfJwyYA" alt=""><figcaption></figcaption></figure>

This guide is getting hella long already, so I won’t bore you with adding more clothes. The process will be the same no matter what you add.

One thing you may want to do is hide some of the body submeshes to prevent clipping through clothes. Find the t0 mesh component in your appearance and toggle off or on the chunkmasks. You can also open the mesh and switch to the preview tab to see which submeshes you may want to hide.

[(full size image)](https://drive.google.com/file/d/15o88bbzFG2Vu_uZR6v28WZ9n5jnFm3NH/view?usp=drive_link)

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfUO7xpdSdx7fjd14QEO2JJvPtYrcuOVUvZKCqHC04tXHqtx8j2cENF45vqr5aL4ORtRpMZoPV4MW16D5kQdmLwiWpRp5JnJ0FCZNcO2oIluUTK4klYsunJ6T3pKtVPztDKqZ-yWA?key=v-1XJeip1aB1Hl1kfJwyYA" alt=""><figcaption></figcaption></figure>

[(full size image)](https://drive.google.com/file/d/1K4ZR8u8VPMCVmoXFn7LJuo-eDQhZaej6/view?usp=drive_link)

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeuHBQKiQcMLEe_-eYkwUfI5I8rnclKNX0WxGnMkgoQ_dbQFQxsCCBLJfUH4UGWD8zFF-EDLBLTQFhu6Jw6pBjp_TrRtXd_J1X24yLZLstYVm7OtKgxwuyKvCg8l52d_3A0YJEeqQ?key=v-1XJeip1aB1Hl1kfJwyYA" alt=""><figcaption></figcaption></figure>

Step 4: The Paperwork

Save the .app file after you’re done updating and adding your clothing. This can take a while sometimes depending on a few different factors. But just wait until it’s done.

Now, we need to tell the game that there’s a new appearance that can be used for the entity. That means we have to update the .ent file. Find that file in your project and click the blue icon to open it.

Right click on any one of the .ent entries and select “Duplicate in array/buffer.” Just like we did when we duplicated the .app appearance, we’ll need to rename it. Rename it to the same name you used for the appearance. Pay close attention to the formatting of the “name” field. You only need to append the new name to the end of the NPV name.

This is what it should look like.

[(full size image)](https://drive.google.com/file/d/1AaPjFtAJAFjZbIpgLnpJ3I7l_vKhZM2g/view?usp=drive_link)

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeMS0fFl7k2xUfnYn_HBfbE6ePoyuaac4OHobtFR6-datZR-h30-HYr9tF-CMj98ubSCDB7r1ZrucMzD_MyG3TtsiOgzKsFsop_76pw97MatxhWTHYzygJA7Cib6fjnOwzovorIBw?key=v-1XJeip1aB1Hl1kfJwyYA" alt=""><figcaption></figcaption></figure>

[(full size image)](https://drive.google.com/file/d/11cr79JQPMKRO8teAsaZkuAo_yFCtwsT6/view?usp=drive_link)

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeHgvVq5HsaXmppYNJgekPJ55N-88UA7h5LjynBETf0FqcSLMPcpjkGJzd_2gwXV-W7_cWivylvxXZKjV-mqnLWH54m5q5xeo0b17CJXlRBygtIxWIXiAFZq0sXZ41lcLJINnBH?key=v-1XJeip1aB1Hl1kfJwyYA" alt=""><figcaption></figcaption></figure>

Save the .ent file.

If you also want it to spawn in AMM, we’ll need to add the appearance to the .lua too. You can do this in any text editor, I use notepad++

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcPu_lLBvjqJ1kOs9KxZF_gzr-FuOlapIEtTJeojx1Wi6oaQXxtBNbwWHctiui7mipxoIU__3TdCzKUQDqFcewq9jO9X5plaNdpmLj8xT_gS6ooEA5KUhcThaxmXovTfPPJ86Vlxw?key=v-1XJeip1aB1Hl1kfJwyYA" alt=""><figcaption></figcaption></figure>

Pay close attention to the formatting of these names!

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfA4WZ_BQgJ5d6vlPE8SMbCz0gHDn19Jy1Mz-mabXZq9XuPOkosoxm3wWiZ-4cCPl-qzLXJRcdww9WzKqKr22NMjDkMf8gruWDJGXC9u5bwXyFZ6w74egFWuXOQ3BnXC_EIAhwkjg?key=v-1XJeip1aB1Hl1kfJwyYA" alt=""><figcaption></figcaption></figure>

And don’t forget the comma!

[(full size image)](https://drive.google.com/file/d/1DVDePE80gfUXCbmcLvV6DKufGJetoBi1/view?usp=drive_link)

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXefDTQwm4vZh76ps3h1ledcLsrFUU3X0nl8LcNQ7r-Dv4vP2s1_iTKPRbJaQLOVuVFCBEW20AVABGtNNAUydlr5RYIROokDEM_1IHMxfgaQpu91LtvDa0UNGVUPlsx-qmweFg1v_Q?key=v-1XJeip1aB1Hl1kfJwyYA" alt=""><figcaption></figcaption></figure>

If you also want the NPV to show up in photomode, you’ll need to regenerate the photomode files. Thankfully, WolvenKit has a way to do this automatically too! [You can find the guide to do that on the wiki.](https://wiki.redmodding.org/cyberpunk-2077-modding/modding-guides/npcs/npv-v-as-custom-npc/npv-amm-nibbles-replacer#step-1-create-photo-mode-files)

#### Step 5: The Finish Line

This guide assumes you’ve never opened WolvenKit in your life so I’m going to show you how to pack the project.

In the top bar, click “Build” then “Pack Project”.

[(full size image)](https://drive.google.com/file/d/1EFnvv33u8Oqwm3LOoNVDG4Q4IwwTCZhr/view?usp=drive_link)

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfcm4d4ovpIAzt-XpEQYSzIq02pp1aDARQxPTTMeKKTiHlTrPCMHiEAkGlJA5v-YXxVoZQ8klVmOeDyzX4zlEvzpSRTJY0Svt9j73wSVaxojUfCOGOaYGaUCuKA4WvsxuvH72GF3Q?key=v-1XJeip1aB1Hl1kfJwyYA" alt=""><figcaption></figcaption></figure>

The log will show you when the packing is complete.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeU0ozEYNNLBCRwZhSaosWMksd0wYTLoZH5JniakqVnjrE9_AAJrfO1Q_ko9xqhIxdV2D2jbW7E6hA7eQx8CQZ5bDruMqgVduMICE52QqSMwEtQdBQb8QM2CC3215BerzvOpxvCiA?key=v-1XJeip1aB1Hl1kfJwyYA" alt=""><figcaption></figcaption></figure>

You can click Build and Install or you can click the yellow folder in the Project Explorer to open the project folder.&#x20;

[(full size image)](https://drive.google.com/file/d/1OSW3rYfG1gyjo1nWMAQEhL1Dih6EBeqs/view?usp=drive_link)

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdDJxKZXh_e1JorxpH_ooagxYsb-3yz5dhQAyEjKUGYjdeWtE5FgQo9fyEt8gK9O6iN_-k3nQdRAikqU36NTXa-7O6u7Loa-9I3MswoX7ggrCSoW_TEossTRWaz3B_y4LVEzj_e?key=v-1XJeip1aB1Hl1kfJwyYA" alt=""><figcaption></figcaption></figure>

\
\
\
\
\
\
\
\
<br>

Go up a level and you’ll find a .zip file with the packed mod, ready to install.

[(full size image)](https://drive.google.com/file/d/18KJ7yX_OoyX9lwFalXQsRWgsboFrbYgC/view?usp=drive_link)

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcEAWClALazReX7nog0kFCNqVprOqgdQPpZC5UV8onp90JV61gILvjkttD5p_oKQQonLd2g9hqFJo6Sgo3SlWWP35vmMtOpN93ueTxBAScn2yyvKCt_VGussTIEqk1SqcNyD_waNA?key=v-1XJeip1aB1Hl1kfJwyYA)

<br>

If you made a new project and aren’t using the one the modder did, make sure you uninstall the old NPV file.

<br>

And that’s it! Install and go, test it out!

<br>

### Final Notes

Garment support doesn’t work on NPVs. You can hide submeshes in ACM or in WolvenKit. You can also edit the mesh(es) in Blender to cut out or resize the parts that clip with other items. I’m too lazy for that and just edit out the clipping in Photoshop lol.

<br>

This process should work for NPC+ too. And again, please don’t hesitate to reach out to me if you need help!
