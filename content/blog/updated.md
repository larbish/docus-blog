---
title: Commodo sed egestas egestas fringilla phasellus
image: /images/blog/three.jpg
tags:
  - sollicitudin
  - aliquam
previewSnippet: >-
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
  incididunt ut labore et dolore magna aliqua. Viverra tellus in hac habitasse
  platea dictumst vestibulum. Lacus sed turpis tincidunt id. Porta lorem mollis
  aliquam ut porttitor leo a diam sollicitudin. Sit amet consectetur adipiscing
  elit ut. Lectus magna fringilla urna porttitor rhoncus dolor purus non enim.
  Lectus sit amet est placerat in. Ipsum dolor sit amet consectetur adipiscing
  elit pellentesque. Accumsan in nisl nisi scelerisque eu. Semper quis lectus
  nulla at volutpat. Id eu nisl nunc mi ipsum faucibus vitae. Dui sapien eget mi
  proin sed libero enim sed.
template: blogpost
---

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Viverra tellus in hac habitasse platea dictumst vestibulum. Lacus sed turpis tincidunt id. Porta lorem mollis aliquam ut porttitor leo a diam sollicitudin. Sit amet consectetur adipiscing elit ut. Lectus magna fringilla urna porttitor rhoncus dolor purus non enim. Lectus sit amet est placerat in. Ipsum dolor sit amet consectetur adipiscing elit pellentesque. Accumsan in nisl nisi scelerisque eu. Semper quis lectus nulla at volutpat. Id eu nisl nunc mi ipsum faucibus vitae. Dui sapien eget mi proin sed libero enim sed.

Tincidunt id aliquet risus feugiat in ante metus dictum. Vehicula ipsum a arcu cursus vitae congue mauris rhoncus. Nisi est sit amet facilisis magna etiam. Tristique senectus et netus et malesuada fames ac turpis egestas. Commodo elit at imperdiet dui accumsan sit amet nulla facilisi. Iaculis urna id volutpat lacus. Tempus imperdiet nulla malesuada pellentesque elit. Rhoncus aenean vel elit scelerisque mauris pellentesque. Odio facilisis mauris sit amet massa vitae tortor condimentum. Eget mauris pharetra et ultrices neque ornare aenean euismod elementum. Bibendum est ultricies integer quis auctor elit sed vulputate. Molestie ac feugiat sed lectus. Diam vel quam elementum pulvinar etiam non quam lacus.

Nec sagittis aliquam malesuada bibendum arcu vitae elementum. Imperdiet sed euismod nisi porta lorem mollis aliquam. Amet purus gravida quis blandit. Amet consectetur adipiscing elit ut aliquam purus. Urna porttitor rhoncus dolor purus non. Tortor consequat id porta nibh venenatis cras sed felis eget. Sit amet cursus sit amet dictum sit amet. Praesent tristique magna sit amet purus gravida quis. Et malesuada fames ac turpis egestas maecenas pharetra. Faucibus a pellentesque sit amet porttitor eget dolor. Nulla aliquet enim tortor at auctor. Pellentesque sit amet porttitor eget. Consequat mauris nunc congue nisi vitae.

```bash
$ npm install wearefractal/vinyl-fs
```

Tortor consequat id porta nibh venenatis cras sed felis eget. Sit amet cursus sit amet dictum sit amet.

```typescript
var fs = require('vinyl-fs'),
  gzip = require('gulp-gzip')

grunt.registerTask('zip', function () {
  fs.src('./build/build.js').pipe(gzip()).pipe(fs.dest('./build')).on('end', this.async())
})
```

Praesent semper feugiat nibh sed pulvinar proin. In fermentum posuere urna nec tincidunt praesent. Nunc scelerisque viverra mauris in aliquam sem. Scelerisque eleifend donec pretium vulputate sapien nec. Eu ultrices vitae auctor eu augue ut lectus arcu. Commodo sed egestas egestas fringilla phasellus. Tristique et egestas quis ipsum suspendisse ultrices gravida dictum. Sed libero enim sed faucibus turpis. Vestibulum rhoncus est pellentesque elit. Lorem sed risus ultricies tristique nulla aliquet enim tortor at. Fermentum leo vel orci porta non pulvinar neque laoreet. Cras pulvinar mattis nunc sed blandit libero volutpat sed. Integer quis auctor elit sed vulputate.

![Example](/images/blog/four.jpg "Example")

Vestibulum rhoncus est pellentesque elit. Lorem sed risus ultricies tristique nulla aliquet enim tortor at.

```typescript
var fs = require('vinyl-fs'),
  map = require('map-stream'),
  zlib = require('zlib')
grunt.registerTask('zip', function () {
  fs.src('./build/build.js').pipe(map(gzip)).pipe(fs.dest('./build')).on('end', this.async())
})
// all you need to do is modify the file's
// contents and then call the callback.
// Just remember it's always buffer in and buffer out.
function gzip(file, cb) {
  zlib.gzip(file.contents, function (err, buffer) {
    file.contents = buffer
    file.path = file.path + '.gz'
    cb(err, file)
  })
}
```

Ut pharetra sit amet aliquam id diam. Purus non enim praesent elementum. Lacus luctus accumsan tortor posuere ac ut. Massa id neque aliquam vestibulum morbi blandit cursus risus at. Nulla aliquet enim tortor at auctor urna. In mollis nunc sed id semper risus in. Sed id semper risus in hendrerit gravida rutrum quisque. Cras tincidunt lobortis feugiat vivamus at augue eget. Metus aliquam eleifend mi in nulla posuere sollicitudin aliquam. Ut lectus arcu bibendum at varius vel pharetra vel. Volutpat blandit aliquam etiam erat. Sit amet risus nullam eget felis eget nunc.
