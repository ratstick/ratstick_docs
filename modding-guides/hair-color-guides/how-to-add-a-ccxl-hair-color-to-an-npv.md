---
description: >-
  This guide will walk you through pathing hair color textures when you want to
  use a CCXL hair color on an NPV or NPC+
---

# How to Add A CCXL Hair Color to an NPV

You’ll just path the .hp and cap files. Some of this is going to be a little funky but don’t worry about it lol. Okay, we’re going to use hh\_043\_wa\_\_modern\_bob.mesh as our example for this one. I want to make sure my NPV is using flecktarn.

### Mesh prep

Since we’re essentially replacing the .hp and cap .xbm, you can pick whichever color you want here.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcbpyPmVQJH3_c1iM1_D_6u3ZU_yaSrgG-9cYegjiOpG-X4Fhy_qL9rYd5BXaK76Ksd-vpzI_Md1uzePkcbwfimuPZXg-DSPuXnhylEpoumXQ6pUzYjfTG4bYWZILrh0wuAp9Qz?key=861_VgN82g7h-lIzl-y5SA" alt=""><figcaption></figcaption></figure>

I’m going to do blonde\_platinum in this instance.

### Pathing the textures

#### .mesh textures

Add the .mi files from the hair mesh as indicated in localMaterialBuffer and/or externalMaterials.&#x20;

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdriyBhTY53c6sqMFIWcq7XxQofaLkbAQMY1iYHcPoLWHUiggi1ATmNpu4VDTd2IBOV-JOPfvZCGqqsAZgOvFCF_Jsp3BYe112Z_pK5IKUZwhAlNvhl9awCG8X-jRSC29uIKUAtXg?key=861_VgN82g7h-lIzl-y5SA" alt=""><figcaption></figcaption></figure>

.mi textures

We have the vanilla blonde\_platinum hair profile in here. We can just replace it with the hair profile you want to use from one of my mods.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcYdQKlkKH0VYEift3-Mm8dQlthpqtsxSYQida6KAdUrZQgeyKxHImN6rBQcQm-eX7-vKpUb4Jan8THWu5LFolRmYr7t4q0lVJXKskBHvRpRsF5eaqnHZZlm6BcAvhlgsmPy9QkaA?key=861_VgN82g7h-lIzl-y5SA" alt=""><figcaption></figcaption></figure>

And that’s it!

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcswQXMPu_qQEcC0BNyL-gdPbnKhLE7f2xXWRCQG8QUkGvvEoTDRUzlkXCJM7WmUO6XkxX0YdzB7oAUkLT6HsymIrbeWRPJ1Yi0YeSfaG3w67N0DEaosAs5fM6RtRYEDwZCWh5PNQ?key=861_VgN82g7h-lIzl-y5SA" alt=""><figcaption></figcaption></figure>

Cap files

The hair above doesn’t need a cap. Let’s look at one that does have a cap to show you how to replace it with my cap.

I’m using the rattail. Here are the initial materials custom pathed:

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdZsieY6arjK2G7yWNpcS9ecFVu-_y5_HB-7aEGhupGBfdrou5rmPRwxrXfnflQpPiGaNprZGI1OMxWvyh5f9jDASNRbBPCUZVGop1a0NYhV7dXvSOmZUJq4SP0lG0gER6Lc2SlVg?key=861_VgN82g7h-lIzl-y5SA" alt=""><figcaption></figcaption></figure>

Just like in the prior section, we’re updating the .hp in the first .mi

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXc7e-ceGeAyTxbl0kifWJsYSgWUQb6-bpBzm4JE3V92kSfYcShjvZXQIK80li_EjFwCgdpZuq2CQnKDw_oNXsBvYUTyOIrlRsq6Ac1K35-f4iwLr8YJzGFhx0p2TFgcBay9oEMG8Q?key=861_VgN82g7h-lIzl-y5SA" alt=""><figcaption></figcaption></figure>

The two values in hh\_026\_black\_carbon\_\_cap.mi are the non-color textures, the ones that dictate the pattern and whether or not you have to use the special cap for cyberware 01. Path these as you normally would either with vanilla or any texture mods you use.&#x20;

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdZzgmWuvU-Q7eamRGCo8vwT8TK9X80xzEkMakGWFtaR52kUsKrblJOte0A_lskxdb8NFAiRKJzOosPlpYedXjDmekoTMUyOQwXgMragI2DnSpePZwHzG3H5_xqY3bgvDXPpLj6EA?key=861_VgN82g7h-lIzl-y5SA" alt=""><figcaption></figcaption></figure>

The file we’re going to edit for the cap color will be in the black\_carbon\_\_cap.mi

Add the hh\_cap\_grad\_\_ file from my mod. In this case, it’s hh\_cap\_grad\_\_flecktarn.xbm

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfuDKMEhtbYd4qmaCFuddCYBS5f1_4NoNgptHlJ9iDKhNUi4PrW5CGYflDoSxys0JOBA0zvE5O6RGZvq3zSKCfwSrz0LPjyA5LxjO4Q29Pho6xlYwb4nN7VeEPxbK2rHyIlCzsXoQ?key=861_VgN82g7h-lIzl-y5SA" alt=""><figcaption></figcaption></figure>

Path it in the cap.mi file

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfETkI5XZD84kARraKBFwZgd7myq77aYqux0xUyxo5NTf2vhXkoNsA4w9QHNkAZq3lGuBqxISZUsatIfmZ6c8S_pla0lg061TZePNunnlcgKDXtLdKjc2VvBQ1BWiox803_VaCf8g?key=861_VgN82g7h-lIzl-y5SA" alt=""><figcaption></figcaption></figure>

Save the file and you’re all set!

### A little theory (if you’re interested)

You can ignore all the other files in my CCXL mod for NPV/NPC+ because CCXL standardized the hair textures, allowing the ability to use dynamic materials.&#x20;

Dynamic materials means being able to use wildcards so you can have multiple textures but only need to path one with wildcards. For example, in my CCXL hair colors, we have these generic .mi files. The paths to the .hp files looks like this: \*ratstick\kermie\_ccxl\hair\_profiles\\{material}.hp

The .mesh and .mi files are just part of the way CCXL works and loads the materials. But the cap .xbm and .hp files are the only ones I’m actually changing. So, we only need to update the files that change the color in the NPV/NPC+
