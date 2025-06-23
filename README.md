# 𝚂𝚘 𝚈𝚘𝚞'𝚟𝚎 𝙰𝚕𝚠𝚊𝚢𝚜 𝚆𝚊𝚗𝚝𝚎𝚍 𝚃𝚢𝚙𝚎𝚠𝚛𝚒𝚝𝚝𝚎𝚗 𝚆𝚎𝚋𝚜𝚒𝚝𝚎...

This quick guide will have you up & running in no time. You will need:

1. Scanned images of your typewritten pages
2. Some software to edit vector graphics
3. SVGo installed globally ( if you are anti `package.json` like myself )

Currently, this framework support links and nothing else.

## Step One : (っ◔◡◔)っ ♥ Preparing The Vectors ♥

You'll need SVGs of your scanned pages. I like Inkscape's bitmap trace for this purpose. Now pull your new vector graphics into your software of choice. This repo is designed around Affinity Designer, as that's what I use. The object here is to make sure anything that should function as a link is its own separate path. You'll also want to add a box underneath your links, which will function as a 'mouse buffer zone' so that clicking is intuitive for your many, many vistors. The box's fill should be set to the background color of your pages/site. Here is an example of some link text with the box beneath it: 

<img width="432" alt="Captura de Pantalla 2025-06-22 a la(s) 8 14 06 p m" src="https://github.com/user-attachments/assets/ad30e79b-f61d-45f6-934b-196392718e38" />

Now, in Affinty Designer, layer names in the software become the `id`s of the corresponding `<g>` tags in the exported SVG. Unless there are duplicate layer names, in which case Affinity prepends a digit to the `id` and adds a new attribute, `serif:id`, with the original layer name to the `<g>`. If you are not using Affinity Designer, you'll need to see the naming conventions of your vector software and edit the code appropriately. In Designer, rename all paths/layers that should function as links like so: `@<YOUR URL HERE>`. The link text and its border box should be named identically. Like so:

<img width="255" alt="Captura de Pantalla 2025-06-22 a la(s) 8 23 46 p m" src="https://github.com/user-attachments/assets/21aa7cac-96f0-4d6d-9054-86434036acf0" />

Export the SVG and head to step No. 2.

## Step Two : ₐₛₛₑₘbₗᵢₙg ₜₕₑ Cₒdₑ

I


