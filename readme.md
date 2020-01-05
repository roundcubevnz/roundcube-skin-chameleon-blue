Chameleon Blue Kolab Roundcube Skin
===============================

Chameleon Blue customization of [Chameleon](https://git.kolab.org/diffusion/RSC/), 
also known as Kolab Enterprise Web Client Skin.


![Kolab Blue](screenshots/preview.png "Preview of Chameleon Blue")

## installation

Merge "skins" folder with your Roundcube instance/skins directory.

**Chameleon depends on Larry, so this skin must be installed too.**

## Hacking

styles.css is written using LESS syntax, compiled with `lessc` by `nodejs-less`
but there's better options like https://github.com/codeigniterpower/compiler-lessphp

 $ lessc -x styles.less > styles.css

(the -x option minifies the CSS code)

References to image files from the included CSS files can be appended
with cache-buster marks to avoid browser caching issues after updating.

Run `bin/updatecss.sh --dir <path-to-chameleonb-skin>` from the Roundcube
package before packaging the skin or after installing it on the
destination system.

# License
blued by Pavel Kosko aka Skolzyashiy
Screendesign and icons by [Kolab Systems AG, Zurich, Switzerland](http://kolabsys.com)

The contents of this folder can be redistributed and/or modified
under the terms of the GNU Affero General Public License as published
by the Free Software Foundation, either version 3 of the License,
or (at your option) any later version.


