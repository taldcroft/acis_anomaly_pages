.. _dea-shutdown:

DEA-A Anomalous Shutdown
========================

What is it?
-----------

The DEA-A shuts down anomalously, presumably due to a spurious command.

When did it happen before?
--------------------------

The DEA-A has shutdown only once in the mission, in 2005:

* September 16, 2005, 2005:259:11:02

Will it happen again?
---------------------

It appears it could happen again, but one occurrence in 16 years provides little guidance.

What is the first response?
---------------------------

Our real-time web pages will alert us and the Lead System Engineer will call us. We need to process the dump data and
make sure that there is nothing anomalous in the data *BEFORE* the shutdown. We want to know if a new occurrence looks
just like the previous occurrences. If yes, it should appear as if in one frame the DEA-A turned off. We need
to process the dump data, send an email to the ACIS team (including Peter Ford, Bob Goeke, Mark Bautz, and Bev LaMarr),
and convene a telecon at the next reasonable moment. A DEA-A recovery requires that the BEP be warmbooted after the
DEA-A is back on (see SOP and Flight Note for details).

Impacts
-------

* Until the DEA is powered back on, science operations will be interrupted.
* After DEA is powered back on, the focal plane temperature will be unregulated and possibly uncalibrated.  Recovery will require a BEP warmboot and setting the focal plane temperature to -121 C.
* The warmboot of the BEP will reset the parameters of the TXINGS patch to their defaults.  They can be updated in the weekly load through a SAR.

Relevant Procedures
-------------------

SOT Procedures
++++++++++++++

* `Turn On DEA-A <http://cxc.cfa.harvard.edu/acis/cmd_seq/deaa_on.pdf>`_
* `Warm Boot the Active ACIS BEP and Start DEA HK Run <http://cxc.cfa.harvard.edu/acis/cmd_seq/warmboot_hkp.pdf>`_
* `Set Focal Plane Temperature to -119.7 C <http://cxc.cfa.harvard.edu/acis/cmd_seq/setfp_m121.pdf>`_

FOT Procedures
++++++++++++++

* `SOP_61036_DEAA_ON <http://occweb.cfa.harvard.edu/occweb/FOT/configuration/procedures/SOP/SOP_61036_DEAA_ON.pdf>`_
* `SOP_ACIS_WARMBOOT_DEAHOUSEKEEPING <http://occweb.cfa.harvard.edu/occweb/FOT/configuration/procedures/SOP/SOP_ACIS_WARMBOOT_DEAHOUSEKEEPING.pdf>`_
* `SOT_SI_SET_ACIS_FP_TEMP_TO_M121C <http://occweb.cfa.harvard.edu/occweb/FOT/configuration/procedures/SOP/SOP_SI_SET_ACIS_FP_TEMP_TO_M121C.pdf>`_

Relevant Notes/Memos
--------------------

* `Flight Note 572 <http://cxc.cfa.harvard.edu/acis/memos/Flight_Note572_DEA_Shutdown_Closeout_merged.pdf>`_
* `ACIS - DEA ADC Reset (Dorothy Gordon) <http://cxc.cfa.harvard.edu/acis/memos/gordon_dea_20051118.pdf>`_