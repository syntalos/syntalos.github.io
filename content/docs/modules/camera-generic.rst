---
title: Generic Camera
---
.. image:: /images/modules-src/camera-generic.svg
   :width: 80
   :align: right

The "Generic Camera" module can connect to any UVC webcam / V4L2 supported device that
can be opened using `OpenCV <https://opencv.org/>`_.
(This sometimes also includes industrial cameras for which no specialized drivers exist).


Usage
=====

Configure as usual.


Ports
=====

.. list-table::
   :widths: 14 10 22 54
   :header-rows: 1

   * - Name
     - Direction
     - Data Type
     - Description

   * - Video🠺
     - Out
     - ``Frame``
     - ~


Stream Metadata
===============

.. list-table::
   :widths: 15 85
   :header-rows: 1

   * - Name
     - Metadata

   * - Video🠺
     - | ``size``: 2D Size, Dimension of generated frames
       | ``framerate``: Double, Target framerate per second.
