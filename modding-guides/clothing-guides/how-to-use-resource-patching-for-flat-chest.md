---
description: >-
  This guide will walk you through how to edit a mod's .xl file so that a mod
  that was only made for the equippable flat chest can also be made to recognize
  the flat chest body. Work smarter not harder!
---

# How to Use Resource Patching for Flat Chest

## What is resource patching?

Resource patching is a function of ArchiveXL that allows you to tell the game to load a specific mesh for a specific body, even if the mesh doesn't exist with that tag. This means you can create a refit just for RB and EBB and use resource patching so both meshes load for EBBRB.

## Why would I want to do this?

Refits can be a bit time consuming depending on if it has a script in the Blender autorefitter and a bit difficult and fiddly depending on weight adjustments. Many modders may limit their refits to a certain set of bodies for multiple reasons. Since the sculpt of the flat chest body and the equippable flat chest are somewhat similar, you can use resource patching to tell the game to load an equippable flat chest refit for the flat chest body.

## Cool, how do I do it?

You only need to add a couple lines of code to your .xl file! Beneath the factories and localization sections, add the following:

{% hint style="info" %}
You'll need to copy the relative path to your mesh for the link section.
{% endhint %}

```
resource:
  link:
    base\modname\itemname_base_body_flat.mesh:
      - base\modname\itemname_flat.mesh
```

Add an entry for every mesh. The finished .xl file should look something like this:

```
factories:
  - base\rat_shirt\axl\rat_shirt_factory.csv
localization:
  onscreens:
    en-us: base\rat_shirt\axl\rat_shirt_local.json

resource:
  link:
    base\rat_shirt\mesh\rat_shirt_base_body_flat.mesh:
      - base\rat_shirt\mesh\rat_mesh_flat.mesh
```

Save the file and go! If you're doing this for a mod that you didn't make, I recommend making a backup of the .xl file with your changes in case the mod updates.
