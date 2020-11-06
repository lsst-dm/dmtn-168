..
  Technote content.

  See https://developer.lsst.io/restructuredtext/style.html
  for a guide to reStructuredText writing.

  Do not put the title, authors or other metadata in this document;
  those are automatically added.

  Use the following syntax for sections:

  Sections
  ========

  and

  Subsections
  -----------

  and

  Subsubsections
  ^^^^^^^^^^^^^^

  To add images, add the image file (png, svg or jpeg preferred) to the
  _static/ directory. The reST syntax for adding the image is

  .. figure:: /_static/filename.ext
     :name: fig-label

     Caption text.

   Run: ``make html`` and ``open _build/html/index.html`` to preview your work.
   See the README at https://github.com/lsst-sqre/lsst-technote-bootstrap or
   this repo's README for more info.

   Feel free to delete this instructional comment.

:tocdepth: 1

.. Please do not modify tocdepth; will be fixed when a new Sphinx theme is shipped.

.. sectnum::

.. TODO: Delete the note below before merging new content to the master branch.

.. note::

   **This technote is not yet published.**

   Notes on running DRP pipelines using PanDA (Production ANd Distributed Analysis system)

.. Add content here.
.. Do not include the document title (it's automatically added from metadata.yaml).
.. .. rubric:: References

.. Make in-text citations with: :cite:`bibkey`.

.. .. bibliography:: local.bib lsstbib/books.bib lsstbib/lsst.bib lsstbib/lsst-dm.bib lsstbib/refs.bib lsstbib/refs_ads.bib
..    :style: lsst_aa

Introduction
============
The PanDA (Production ANd Distributed Analysis) is a multi-component workload management system for distributed (GRID
based), Cloud, or HPC computing. PanDA based setups usually include few leveraged components such as:

- PanDA server + JEDI [PanDA_twiki]_, [PanDA_paper]_
- JEDI system [JEDI_twiki]_
- Harvester [Harvester_slides]_, [Harvester_paper]_
- Pilot [Pilot_paper]_
- iDDS [iDDS_slides]_
- Monitoring [monitoring_paper]_
- CRIC [CRIC_slides]_

All these components have a well-defined scope of functionality and its independent installation allows to manage deeply
customized instances.
For the year 2019 the ATLAS PanDA instance landed 394M computing jobs on 165 computation queues distributed all over the World.
There are more than 3000 users use BigPanDA monitor. PanDA system has been successfully adopted by other experiments,
e.g. COMPASS [compass_paper]_
In this note we describe processing the HSC-RC2 dataset within the DRP pipeline and PanDA based workload management setup.

Setup
=====

Workflow generation
===================

Data Processing
===============

Conclusion
==========

References
==========

.. [PanDA_twiki] PanDA Twiki Page `https://twiki.cern.ch/twiki/bin/view/PanDA/PanDA <https://twiki.cern.ch/twiki/bin/view/PanDA/PanDA>`_
.. [PanDA_paper] Evolution of the ATLAS PanDA workload management system for exascale computational science `<https://www.researchgate.net/publication/274619051_Evolution_of_the_ATLAS_PanDA_workload_management_system_for_exascale_computational_science>`_
.. [JEDI_twiki] JEDI Twiki Page `<https://twiki.cern.ch/twiki/bin/view/PanDA/PandaJEDI>`_
.. [Harvester_slides] Harvester Slides `<http://cds.cern.ch/record/2625435/files/ATL-SOFT-SLIDE-2018-400.pdf>`_
.. [Harvester_paper] Harvester: an edge service harvesting heterogeneous resources for ATLAS `<https://www.epj-conferences.org/articles/epjconf/pdf/2019/19/epjconf_chep2018_03030.pdf>`_
.. [Pilot_paper] The next generation PanDA Pilot for and beyond the ATLAS experiment `<https://cds.cern.ch/record/2648507/files/Fulltext.pdf>`_
.. [iDDS_slides] iDDS slides `<https://indico.cern.ch/event/849155/contributions/3576915/attachments/1917085/3170006/idds_20100927_atlas_sc_week.pdf>`_
.. [monitoring_paper] BigPanDA monitoring paper `<https://inspirehep.net/files/37c79d51eadd0e8ec8e019aef8bbcfd8>`_
.. [CRIC_slides] `<https://indico.cern.ch/event/578991/contributions/2738744/attachments/1538768/2412065/20171011_GDB_CRIC_sameNEC.pdf>`_
.. [compass_paper] `<http://ceur-ws.org/Vol-1787/385-388-paper-67.pdf>`_