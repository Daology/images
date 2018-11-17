Place to store images.

SVG can be converted to PNG with:

```bash
for i in *; do rsvg-convert $i -d 300 -p 300 -w 1000 -h 1000 -o `echo $i | sed -e 's/svg$/png/'`; done
```