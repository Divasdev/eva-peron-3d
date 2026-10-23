# Eva Perón — 3D portrait

A full 3D head-and-shoulders portrait of Eva Perón (Evita), made for the assignment
"Reconstruct a Famous Face in 3D".

- **Model (binary glTF 2.0):** https://divasdev.github.io/eva-peron-3d/eva_peron.glb
- **Viewer:** https://divasdev.github.io/eva-peron-3d/

The model is a single `.glb` file under 2 MB with no glTF extensions, so it loads in
any glTF 2.0 viewer (three.js, model-viewer, Blender, Babylon.js).

## How it was made

The head is the ICT FaceKit morphable head, fitted to MediaPipe face landmarks in the
reference photograph (and, for depth, in three more authentic photographs of her), then
corrected vertex by vertex so the features land on the photo exactly. The photo is
projected onto the fitted head as the texture; the side the photo cannot see is completed
by mirroring. Hair (swept back into a loose roll, lengths to the shoulders) and the coat
are modelled as signed-distance volumes. Colour comes from a period colour portrait;
brightness stays exactly as in the photograph.

## Credits

- 3D portrait by Divas Sharma.
- Reference photograph: *Evita* by Pinélides Fusco, late 1948, courtesy Museo Evita, public
  domain, via [Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Evita_(cropped2).JPG).
- Base head topology and shape space: [ICT FaceKit](https://github.com/USC-ICT/ICT-FaceKit),
  © 2020 USC Institute for Creative Technologies, MIT licence (see `LICENSE-ICT-FaceKit.txt`).
- Viewer: [three.js](https://threejs.org) r160 (MIT).
