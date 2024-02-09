# Three.js Minified + Addons

Place `three.min.js` (and `three-addons.min.js` for cool features) in `{_dir}/` to import as `script:src` in `index.html`.

```html
<script src="{_dir}/three.min.js"></script>
<script src="{_dir}/three-addons.min.js"></script>
```

Refer to namespaces `THREE` and `THREE_ADDONS` respectively.

```js
const geometry = new THREE.BoxGeometry(1, 1, 1);
const material = new THREE.MeshStandardMaterial({ color: 0xcccccc });
const cube = new THREE.Mesh(geometry, material);
scene.add(cube);
```

```js
const geometry = new THREE_ADDONS.RoundedBoxGeometry(1, 1, 1);
const material = new THREE.MeshStandardMaterial({ color: 0xcccccc });
const cube = new THREE.Mesh(geometry, material);
scene.add(cube);
```
