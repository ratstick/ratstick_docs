---
description: >-
  This guide will walk you through how to create a replacer version of a CCXL
  hair colors.
---

# How to Convert a CCXL Hair Color Into a Replacer

#### Considerations <a href="#docs-internal-guid-e068ac9f-7fff-7ae9-d8ab-29ff3b1ae3a0" id="docs-internal-guid-e068ac9f-7fff-7ae9-d8ab-29ff3b1ae3a0"></a>

The great thing about CCXL hair colors is that you can create your own cap colors. If you want to convert them to a replacer, then you’ll want to consider the cap color of the vanilla hair color. Replacers will impact anything using that hair profile, I’d recommend staying away from brown\_liquorice and black\_carbon.

You also can only have one replacer installed at a time per vanilla hair color.

#### Reference - Color Names

To make it easy to set up the folder structure for a replacer, you can search for the vanilla hair profile, add it to your project, and then just rename and overwrite the mod file. Here’s a list of all the vanilla .hp profiles for easy reference. (“liliac” is not a typo). You can use the screenshot from the wiki [Cheat Sheet: Hair ](https://wiki.redmodding.org/cyberpunk-2077-modding/for-mod-creators-theory/references-lists-and-overviews/cheat-sheet-head/hair#colour-in-files-by-index)article for reference. These are the colors you can replace.

If you want to set up the path yourself, here it is:

`base\characters\common\hair\textures\hair_profiles\`<br>

| brown\_liquorice       | blonde\_platinum | red\_merlot         | ginger\_copper    |
| ---------------------- | ---------------- | ------------------- | ----------------- |
| teal\_ombre            | black\_carbon    | blonde\_golden      | blonde\_dishwater |
| blue\_sapphire         | brown\_ombre     | red\_apple          | gray\_gunmetal    |
| ginger\_strawberry     | teal\_ash        | pink\_magenta       | pink\_rose        |
| blue\_steel            | blue\_red\_ombre | cold\_white         | cyberpunk\_yellow |
| goblin\_green          | liliac           | mermaid\_aquamarine | purple\_ombre     |
| black\_salt\_n\_pepper | green\_toxic     | brown\_medium       | blue\_sky         |
| citrus\_yellow         | dark\_purple     | green\_orange       | liliac\_ombre     |
| phoenix\_fire          | purple\_blonde   | silver\_rose        | <p><br></p>       |

[Step 0: Create a WolvenKit project](https://wiki.redmodding.org/wolvenkit/getting-started/creating-a-mod#getting-started-with-wolvenkit)

#### Step 1: Folder structure

Because we are replacing a vanilla hair profile, we need to mirror the vanilla folder structure in our project. In the asset browser, search for the hair profile you want to replace.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfK8_oUydO1eV6k-ZRw7NwzLF-bwhHFz174I0eqE-0gJW_hUKQfeSVhFvQbSvubwWlnY8tyiKtTjhcS8xlXGv2weOPTvxZVqZpYU6mHKbrfEunrBH-KwswJXsUA5XvnpVmZs2fxRg?key=861_VgN82g7h-lIzl-y5SA" alt=""><figcaption></figcaption></figure>

Right click, and select “add selected items to project.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfIZuOM7UMCDYzZ--xseQooDlCL2L0R2bKKqSEvcqZFuXXDui1ty4EIX3YdTl9bjIwndhaE_BN8xftvRQF2lQk2vajXJJjUppX3ctC9QJNZ8E8m57PT8M452KE3VgA5MRtoOEdxvQ?key=861_VgN82g7h-lIzl-y5SA" alt=""><figcaption></figcaption></figure>

You should now see this in the Project Explorer on the left.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfIqMYfC4jgmVajO_7CIndt5g1DTwnXNliKlhU2kAzKRw7bA4WgYVCXGXhsodiFf0NE8WY24cVqKa8HoLxKbgBy1d7-2C3GiuOFymNDG-c0_pTXZHJSrBjvrKrdwVWFAvF3nAJd?key=861_VgN82g7h-lIzl-y5SA" alt=""><figcaption></figcaption></figure>

Step 2: Finding one of my hair profiles

CCXL hair colors all use the same folder structure. You’ll find all of mine here:

`ratstick\modname_ccxl\hair_profiles`

Use the reference pics on the mod page to find the color name. For this example, I want to replace brown\_medium.hp with the color “flecktarn” from my [It Ain’t Easy Bein’ Green](https://www.nexusmods.com/cyberpunk2077/mods/22271) pack.

Toggle the asset browser to the mod browser and search for “ratstick”

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeH-FIlGvy--md9VNVxb3Zm7ICNarXLs0LzkmrsCK2BMaOBG53TCtNyxmcPO0hHtVdtIusawIgUw6Nci0aefG55RhgGRRhUaD8a9NeAribsEOMW_aXs_nEtzDnVhUoyezRRxfQ4?key=861_VgN82g7h-lIzl-y5SA" alt=""><figcaption></figcaption></figure>

I’m going to uncheck “select all” and then check “ratstickkermie\_ccxl.archive”, just to make it easier to navigate. You can also try searching for the .hp name without filtering. Most of my colors are named the same as in the hair profile and in the reference photos.&#x20;

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdoVhweIJL8zS70dlWSXVZIc9cDEXTFobSIYondd_va4l3rdfeF2FcQX83jk79rK621NeObd8PWCfy6pNQlySEwbfjv2pZWzBndMJAsejsNH6lTjWi1hrBoTS495NTZuTVL6_M8Jw?key=861_VgN82g7h-lIzl-y5SA" alt=""><figcaption></figcaption></figure>

Right click on the .hp you want to add, in this case flecktarn.hp, and click “Add selected item to project.”

This is what you should see on the left in your Project Explorer.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdhCa0MCvPuxvzP1DRlmbqcFvjhHcEpGb6Bq64OE0-doYSlm7e9HmR4vncsR_N92Lsp6z7Rv5bU7sDwl8tWtmNWyoVs3mrLV140OtwxW_zNO5TSGjXUOsKLMXxvZpHMV3R1NdC9?key=861_VgN82g7h-lIzl-y5SA" alt=""><figcaption></figcaption></figure>

Step 3: Rename and move the file

Now, rename the hair color from my mod to the color you’re replacing.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfPdfgiDog0vX5Ayzb9uYzbtQ6bFxnM2iTBHOs2inHUmOOF48PZuKmXwkyi_c9yGRSgjwJEw_mpAuNo6WB1APKbcIYkewtvfir89bL51tnZ0a-ImxK7tYFnOyb7xGy2eX4QcCTx1Q?key=861_VgN82g7h-lIzl-y5SA" alt=""><figcaption></figcaption></figure>

Your project explorer should now look like this:

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcaqX8HYJiwRThcl7HWM8o_1j6MU_g3NTH2yia4DQAVKCPVPCB7Es0YM5W7i_sCk7FEJZw59oWzbj-uaEYNL7kBF-s2M1Pp5THkr29Iexd_ZA1LtmE4itCcDa5up1B8A5mvYfhOBg?key=861_VgN82g7h-lIzl-y5SA" alt=""><figcaption></figcaption></figure>

All that’s left is to drag and drop into our vanilla folder and let it replace the vanilla file.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXf-o84uT_K61kqulhbDKXbI5FM0RwZF_p_aHb3y8p6H3GuZG2zqLzMHCM1J1IXpEZeNb6IhVyhyvcssDekfKO8J5r3H_VFfJp-QkU7Udhv0e22a3N3LIXHijF5UPzZ--jEGY1AkQg?key=861_VgN82g7h-lIzl-y5SA" alt=""><figcaption></figcaption></figure>

Project Explorer should look like this now:

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXf90IcV0PQ3m93IRHuzaHWUQ5h-ajblJG0tBvg_OO73xlfGE2uen5yWtK5FceuSJAwcqrEPQ-AYBwK5NUWB11UPfXun6tA65s8Zz5GWp8w6LxOKkxNNX-y1E8SO1cWyXAsaQ0RhJw?key=861_VgN82g7h-lIzl-y5SA" alt=""><figcaption></figcaption></figure>

\
Feel free to delete the folders leftover from my mod. Then, just pack, install, and go!
