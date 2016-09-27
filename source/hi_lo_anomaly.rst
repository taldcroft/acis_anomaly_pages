.. _hi-lo-anomaly:

Hi/Lo Pixel Anomaly
===================

What is it?
-----------

Event data stops being reported for one CCD/FEP combination and the delta overclock values are peculiar, large and
negative for the first three output nodes and large and positive for the fourth output node.

When did it happen before?
--------------------------

Twice once in 2011 and once in 2013.

Will it happen again?
---------------------

It appears likely it could happen again.

What is the first response?
---------------------------

Most likely we will be notified by CXCDS Ops that data ceased prematurely for a single CCD for an observation. But there
is a chance we can catch this anomaly in a realtime contact during a long observation. If yes, we have a a SOP
(|sop_diagnostics|_) written to intervene if the observation with the anomaly is still in progress to
dump diagnostic data. If not, we need to process the dump data and get access to the CXC products, send an email to the
ACIS team (including Peter Ford, Bob Goeke, Mark Bautz, and Bev LaMarr), and convene a telecon at the next reasonable
moment. We should examine data from the next observation because the setup for the next observation should clear the
problem.

.. |sop_diagnostics| replace:: ``SOP_ACIS_DEA_FEP_DIAGNOSTICS``
.. _sop_diagnostics: http://occweb.cfa.harvard.edu/occweb/FOT/configuration/procedures/SOP/SOP_ACIS_DEA_FEP_DIAGNOSTICS.pdf

Impacts
-------

* The last portion of the science run for that particular CCD/FEP combination will be lost. The following science run
should be unaffected.

Relevant Procedures
-------------------

SOT Procedures
++++++++++++++

* `DEA and FEP Diagnostics Procedure <http://cxc.cfa.harvard.edu/acis/cmd_seq/dea_fep_diags.ps>`_

FOT Procedures
++++++++++++++

* |sop_diagnostics|_

Relevant Notes/Memos
--------------------

* `Hi/Lo Pixel Anomaly Closeout Report <http://cxc.cfa.harvard.edu/acis/memos/OCCcm09291_DDTS_Closeout.txt>`_
* `The ACIS Hi-Lo Pixel Anomaly <ftp://acis.mit.edu/pub/hi-lo-pixel-anomaly-v1.4.pdf>`_