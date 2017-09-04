# SVGRenderer
The SVGRenderer Add-On Widget allowes to create incrediable UI interface elements for the Mendix platform.

## Using the SVGRenderer is very easy.

You need:

1. A microflow that gives a (non) persistent entity back with:
    - An attribute containting the SVG code.
    - A state name attribute.
    - The attributes that the values need to be replaced inside the SVG.

2. The attribute names that can be replaced inside the SVG have to be written in the SVG file as so:

   ```
   [[ attributeName ]]
   ```

The SVG rendering will render the SVG in a container. Setting the "width" and "height" attribute on the SVG tag to 100% will make the SVG responsive even in its own viewport.

SVG's are extreemly powerful instruments to visualize complex user interface elements.

  
