########
Examples
########

Built-in Geometry
=================

This is an example showing how to create a mesh of a simple skrew using the built-in geometry module:

.. image:: https://nschloe.github.io/pygmsh/screw.png
   :align: center

To create the above mesh, simply do:

:download:`Download file <./examples/built_in_tut1.py>`

.. literalinclude:: ./examples/built_in_tut1.py
   :language: python
   :linenos:

to retrieve all points and cells of the mesh for the specified geometry.
To store the mesh, you can use `meshio <https://pypi.org/project/meshio>`_;
for example::

  import meshio
  meshio.write('test.vtu', points, cells, cell_data=cell_data)

The output file can be visualized with various tools, e.g.,
`ParaView <https://www.paraview.org/>`_.

You will find the above mesh in the directory
`test/ <https://github.com/nschloe/pygmsh/tree/master/test/>`_ along with other
small examples.




OpenCASCADE Geometry
====================

As of version 3.0, Gmsh supports OpenCASCADE, allowing for a CAD-style geometry specification.

This is an example showing how to create a mesh of a simple puzzle piece using the OpenCASCADE geometry module:

.. image:: https://nschloe.github.io/pygmsh/puzzle.png
   :align: center

To create the above mesh, simply do:

:download:`Download file <./examples/built_in_tut1.py>`

.. literalinclude:: ./examples/open_cascade_tut1.py
   :language: python
   :linenos:
