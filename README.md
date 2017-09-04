#SVGRenderer

The Scalable Vector Graphics (SVG) Renderer Add-On Widget allows you to create incredible UI interface elements for usage within the Mendix platform.

#Using the SVGRenderer is very easy.

You need:

1. A microflow that returns a (non) persistent entity containing the following attributes:

- An attribute containing the SVG code.  *Format String*

Example:

```
<svg width="100%" height="100%" viewBox="0 0 600 600" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" xml:space="preserve" style="fill-rule:evenodd;clip-rule:evenodd;stroke-linejoin:round;stroke-miterlimit:1.41421;"><g><path id="node1" d="M168.5,162.2c-26,1.4 -52.1,10.7 -74.9,26.5c-9.6,6.7 -29.3,26.1 -35.7,35.3c-2.6,3.6 -6.3,9.6 -8.4,13.5c-2.1,3.8 -4.1,7.4 -4.5,8c-2.9,4.5 -10,25.3 -12.6,37.5c-2.9,13.3 -2.7,43.9 0.4,58c3,13.7 5.6,21.4 10.9,33c9.1,19.8 14.2,26 21,26c6.8,0 13.5,-8.2 11.4,-14c-0.9,-2.9 -0.8,-3 6.9,-7.4c4.3,-2.5 8.6,-5.6 9.4,-6.8c2.3,-3.3 2,-8.2 -0.8,-11.5c-3.6,-4.2 -8.3,-3.8 -17.4,1.5c-4.1,2.3 -7.7,4.2 -8,4.2c-0.4,0 -2.3,-4.2 -4.4,-9.3c-3.8,-9.6 -7.8,-26.2 -7.8,-32.2l0,-3.5l9.4,0c8.6,0 9.7,-0.2 12.4,-2.5c3.8,-3.2 4.7,-6.7 2.7,-10.4c-2.6,-5.2 -5,-6.1 -15.2,-6.1l-9.3,0l0,-3.9c0,-9.3 9.7,-41.1 12.5,-41.1c0.5,0 2.4,0.9 4,2.1c5.4,3.6 12.4,6.9 14.9,6.9c1.3,0 3.8,-1.2 5.5,-2.6c2.4,-2 3.1,-3.4 3.1,-6.1c0,-5.2 -1.3,-6.8 -10,-12c-4.4,-2.6 -8,-5.2 -8,-5.7c0,-3.2 22.8,-26.9 29.7,-30.8l3.1,-1.8l4.5,7.8c5.2,9 6.3,10.1 11.1,10.9c3,0.5 4,0.1 6.6,-2.5c4.5,-4.5 4.1,-8.6 -1.5,-18c-2.5,-4.1 -4.3,-7.7 -4.1,-7.9c0.2,-0.3 3.7,-1.8 7.7,-3.4c9,-3.7 24.7,-7.6 31.9,-8.1l5.5,-0.3l0.3,9.5c0.3,11 1.2,13.5 5.9,15.1c4.2,1.3 7.6,0.6 10.3,-2.3c1.7,-1.9 2,-3.5 2,-12.5l0,-10.4l5.3,0.7c11.9,1.4 33.9,7.7 39.5,11.2c0.9,0.7 0.1,2.7 -3.3,8.4c-5.3,8.8 -5.8,13.2 -2.1,17.5c1.9,2.2 3.2,2.8 6.6,2.8c3.6,0 4.7,-0.6 7,-3.3c1.5,-1.8 4,-6 5.6,-9.2c1.6,-3.2 3.2,-5.9 3.6,-5.9c1.6,-0.2 13.1,9.5 20.4,17.1c12.5,13.1 22.3,28.9 27.9,45.1c3,8.8 6.5,24.5 6.5,29.1l0,3.4l-9.9,0.4c-8.2,0.2 -10.3,0.6 -12.1,2.3c-3.6,3.3 -4.3,6.4 -2.5,10.6c2.2,4.9 4.9,5.9 15.5,5.9l9,0l0,3.6c0,4.5 -4.3,23.4 -6.9,29.9c-4,10.2 -4.6,11.5 -5.4,11.5c-0.5,0 -4.1,-1.9 -8,-4.2c-8.8,-5.3 -13.7,-5.7 -17.3,-1.5c-2.8,3.3 -3.2,8.2 -0.9,11.5c0.9,1.2 3.7,3.4 6.3,4.8c11.7,6.7 11.2,6.2 10.1,9.3c-2.1,6.1 4.5,14.1 11.6,14.1c6.6,0 11.1,-5.5 20,-24.5c5.8,-12.3 8.2,-19.3 11.6,-34c2.1,-8.8 2.4,-12.4 2.3,-30.5c0,-17.7 -0.3,-21.8 -2.2,-30c-3.6,-15.3 -9.1,-30.4 -14.2,-39.1c-1.7,-2.7 -3,-5.2 -3,-5.5c0,-0.2 -1.2,-2.3 -2.7,-4.7c-10.7,-16.5 -28.1,-34.5 -43,-44.4c-11.2,-7.4 -27.1,-15.3 -37.8,-18.6c-17.9,-5.7 -36.3,-7.7 -58,-6.5Z" style="fill:#f42f2f;fill-rule:nonzero;"/><path id="node2" d="M265.4,258.8c-4.5,2 -9.5,4.2 -11,4.9c-16.5,6.9 -25.6,10.8 -28.9,12.3c-2.2,1 -6.9,3 -10.5,4.5c-3.6,1.5 -7.8,3.3 -9.5,4c-16.2,7.2 -17.3,7.5 -21.4,6.6c-8.8,-1.9 -18.4,2.6 -22.7,10.9c-9.3,17.6 10.3,37.4 28,28.3c4.9,-2.5 9.4,-8 11.2,-13.6c0.7,-2.1 10.2,-9.8 38.4,-31c20.5,-15.5 37.6,-28.8 37.8,-29.5c0.6,-2 -2.9,-1.2 -11.4,2.6Z" style="fill:#353535;fill-rule:nonzero;"/><path id="node3" d="M128.5,393.8c-5.7,3.5 -6,4.4 -6.3,19.8c-0.4,15.7 0.5,19.6 5.6,23.1c2.5,1.7 6.1,1.8 52.2,1.8c55.2,0 53,0.3 56.4,-6.8c1.2,-2.7 1.6,-6.5 1.6,-16.9c0,-14.8 -0.7,-17 -5.9,-20.5l-3.4,-2.3l-48.6,0c-45.4,0 -48.8,0.1 -51.6,1.8Z" style="fill:#353535;fill-rule:nonzero;"/><text x="355.263px" y="331.92px" style="font-family:'ArialNova-Bold', 'Arial Nova', sans-serif;font-weight:700;font-size:102.631px;fill:#353535;">[[ amount ]]</text><text x="535.263px" y="257.709px" style="font-family:'ArialMT', 'Arial', sans-serif;font-size:24px;fill:#353535;">[[ indication ]]</text></g></svg>
```

You can get the SVG code by opening an SVG file in your text editor.
Please remove the <!DOCTYPE> attribute at the top of the SVG file.

- A state name attribute. *Format String* 

- The attributes that the values need to be replaced with inside the SVG. *Format String*

2. The attribute names that can be replaced inside the SVG have to be written in the SVG file within double brackets, like:
  
```   [[ attributeName ]]   ```

The SVG rendering will render the SVG in a container. Setting the "width" and "height" attribute on the SVG tag to 100% will make the SVG responsive even in its own viewport.

SVG's are extremely powerful instruments to visualize complex user interface elements.