PASCAL VOC PascalVoc
=================

This library can be used to create image annotation XML files in the PASCAL VOC
file format.

Install
-------

``pip install pascal-voc-pv``

Use
---

    from pascal_voc_writer import PascalVoc

    # PascalVoc(path, width, height)

    pv = PascalVoc('path/to/img.jpg', 800, 400)


    # ::add_object(name, xmin, ymin, xmax, ymax)

    pv.add_object('cat', 100, 100, 200, 200)

    # ::save(path)

    pv.save('path/to/img.xml')

    # ::metadata

    metadata: dict = pv.metadata

    # ::xml_string

    xml: str = pv.xml_string

    
