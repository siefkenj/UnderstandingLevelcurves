# UnderstandingLevelcurves
Activities for understanding and gaining intuition for level curves for functions from R^2 to R

### Surface to Level Curves
Given a physical surface (like those contained in the `models` directory), students should be able to come up with the idea of level curves on their own.  _Wikki Stix_ are like waxy pipecleaners.  They can stick to themselves and paper.  Given Wikki Stix and a 3d printout of one of the models, students should be able to find a 2d representation of them model by phisically manipulating the objects.

### Level curves to Surface
Given level curves, students should be able to mould a surface corresponding to the one being described by level curves using _Playdough_ or clay.


## Development
The models are developed in `openscad`, a computer language for describing solid 3d figures.  The figures are exported through `openscad` to the `.stl` format used by most 3D printers.  If you are on linux, you may batch convert the `.scad` files to `.stl` files with the command

    for i in shape-0*.scad
    do 
      openscad -o ${i%.scad}.stl -D "resolution=1500; size_of_base_in_milimeters = 100" $i
    done

Long Wikki Stix can be obtained here: http://www.officedepot.com/a/products/877958/Wikki-Stix-Super-Wikki-Stix-3/
