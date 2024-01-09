# My 3D Portfolio Website

## Draco 3D Data Compression

Draco is an open-source library for compressing and decompressing 3D geometric meshes and point clouds. It is intended to improve the storage and transmission of 3D graphics.

[Website](https://google.github.io/draco/) | [GitHub](https://github.com/google/draco)

## Contents

This folder contains three utilities:

* `draco_decoder.js` — Emscripten-compiled decoder, compatible with any modern browser.
* `draco_decoder.wasm` — WebAssembly decoder, compatible with newer browsers and devices.
* `draco_wasm_wrapper.js` — JavaScript wrapper for the WASM decoder.

Each file is provided in two variations:

* **Default:** Latest stable builds, tracking the project's [master branch](https://github.com/google/draco).
* **glTF:** Builds targeted by the [glTF mesh compression extension](https://github.com/KhronosGroup/glTF/tree/master/extensions/2.0/Khronos/KHR_draco_mesh_compression), tracking the [corresponding Draco branch](https://github.com/google/draco/tree/gltf_2.0_draco_extension).

Either variation may be used with `THREE.DRACOLoader`:

```js
var dracoLoader = new THREE.DRACOLoader();
dracoLoader.setDecoderPath('path/to/decoders/');
dracoLoader.setDecoderConfig({type: 'js'}); // (Optional) Override detection of WASM support.
```

Further [documentation on GitHub](https://github.com/google/draco/tree/master/javascript/example#static-loading-javascript-decoder).

<h3 align="left"> Connect with me:</h3>
<div align="left">
  <a href="mailto:smayour82@gmail.com">
    <img src="https://img.shields.io/badge/Mail-Contact-informational?style=for-the-badge&logo=gmail" alt="Mail" />
  </a>
  <a href="https://mayourbukhari.github.io/Personal-Portfolio">
    <img src="https://img.shields.io/badge/Visit%20Website-Portfolio-blue?style=for-the-badge" alt="Visit Website" />
  </a>
  <a href="https://www.linkedin.com/in/syed-mohsin-bukhari/">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin" alt="LinkedIn" />
  </a>
  <a href="https://twitter.com/ArraySurvey">
    <img src="https://img.shields.io/badge/Twitter-Follow-blue?style=for-the-badge&logo=twitter" alt="Twitter" />
  </a>
  <a href="https://github.com/mayourbukhari">
    <img src="https://img.shields.io/badge/GitHub-Follow-blue?style=for-the-badge&logo=github" alt="GitHub" />
  </a>
  <a href="https://www.instagram.com/mayour_writes">
    <img src="https://img.shields.io/badge/Instagram-Follow-red?style=for-the-badge&logo=instagram" alt="Instagram" />
  </a>
  <a href="https://kaggle.com/mayourbukhari">
    <img src="https://img.shields.io/badge/Kaggle-Profile-blue?style=for-the-badge&logo=kaggle" alt="Kaggle" />
  </a>
</div>


## License

[Apache License 2.0](https://github.com/google/draco/blob/master/LICENSE)
