LArSoft v05\_15\_01 Release Notes
======================================================================

-   **Table of contents**
-   [LArSoft v05\_15\_01 Release Notes](#LArSoft-v05_15_01-Release-Notes)
    -   [Purpose](#Purpose)
    -   [New features](#New-features)
    -   [Bug fixes](#Bug-fixes)
    -   [Updated dependencies](#Updated-dependencies)
-   [Change List](#Change-List)
    -   [larsoft v05\_15\_01](#larsoft-v05_15_01)
    -   [lareventdisplay v05\_08\_01](#lareventdisplay-v05_08_01)
    -   [larexamples v05\_08\_01](#larexamples-v05_08_01)
    -   [larpandora v05\_09\_11](#larpandora-v05_09_11)
    -   [larana v05\_10\_00](#larana-v05_10_00)
    -   [larreco v05\_14\_01](#larreco-v05_14_01)
    -   [larsim v05\_15\_00](#larsim-v05_15_00)
    -   [larevt v05\_07\_05](#larevt-v05_07_05)
    -   [lardata v05\_10\_00](#lardata-v05_10_00)
    -   [larcore v05\_08\_02](#larcore-v05_08_02)
    -   [larbatch v01\_23\_02](#larbatch-v01_23_02)
    -   [larutils v1\_06\_06](#larutils-v1_06_06)

[list of LArSoft releases](LArSoft_release_list)\
[Download instructions](http://scisoft.fnal.gov/scisoft/bundles/larsoft/v05_15_01/larsoft-v05_15_01.html)

Purpose
--------------------

-   Final release in the v05 series
-   Changes to develop since v05\_15\_00

New features
------------------------------

Bug fixes
------------------------

Updated dependencies
----------------------------------------------

Change List
============================

larsoft v05\_15\_01
------------------------------------------

-   2016-07-19 Lynn Garren : larsoft v05\_15\_01

lareventdisplay v05\_08\_01
----------------------------------------------------------

-   2016-07-19 Lynn Garren : lareventdisplay v05\_08\_01
-   2016-07-16 dorota : Merge branch ‘develop’ of ssh://cdcvs.fnal.gov/cvs/projects/lareventdisplay into develop
-   2016-07-16 dorota : draw 3d trajectories only inside readout-window

larexamples v05\_08\_01
--------------------------------------------------

larpandora v05\_09\_11
------------------------------------------------

-   2016-07-19 Lynn Garren : larpandora v05\_09\_11

larana v05\_10\_00
----------------------------------------

-   2016-07-19 Lynn Garren : larana v05\_10\_00
-   2016-07-16 Kevin Wood : Merge branch ‘develop’ of ssh://cdcvs.fnal.gov/cvs/projects/larana into develop
-   2016-07-15 Kevin Wood : Pass vector arguments into functions via constant references
-   2016-07-14 Kevin Wood : Implemented previous changes in a backward compatible manner
-   2016-07-13 Kevin Wood : Set default value for the (newly implemented) shift variable for OpHit calibration to 0
-   2016-07-13 Kevin Wood : Implemented a shift variable for OpHit calibration

larreco v05\_14\_01
------------------------------------------

-   2016-07-19 Lynn Garren : larreco v05\_14\_01
-   2016-07-18 Alison Roeth : Fix signed/unsigned integer comparison bug in DisambigCheater\_module
-   2016-07-15 Tyler Alion : Allow the DisambigCheater to correct for large ammounts of transverse drift of the electrons due to space charge.
-   2016-07-15 Robert Sulej : cleanup mistakes that Tingjun found
-   2016-07-15 Robert Sulej : quick fix for hit and cluster label names, befor it is reorganised in splitted pma modules
-   2016-07-14 Robert Sulej : Merge branch ‘develop’ of ssh://cdcvs.fnal.gov/cvs/projects/larreco into develop
-   2016-07-11 Robert Sulej : Merge branch ‘develop’ of ssh://cdcvs.fnal.gov/cvs/projects/larreco into develop
-   2016-07-11 Robert Sulej : Merge branch ‘feature/rnd\_ImagePatterns’ into develop
-   2016-06-27 Robert Sulej : Merge branch ‘develop’ into feature/rnd\_ImagePatterns
-   2016-06-24 Robert Sulej : Merge branch ‘develop’ of ssh://cdcvs.fnal.gov/cvs/projects/larreco into develop
-   2016-06-24 Robert Sulej : try code using PtrMaker from Saba (commented out for the moment)

larsim v05\_15\_00
----------------------------------------

larevt v05\_07\_05
----------------------------------------

lardata v05\_10\_00
------------------------------------------

larcore v05\_08\_02
------------------------------------------

larbatch v01\_23\_02
--------------------------------------------

-   2016-07-19 Lynn Garren : Merge branch ‘release/v05\_15\_01’
-   2016-07-19 Lynn Garren : larbatch v01\_23\_02
-   2016-07-19 Herbert Greenlee : Add –jobsub-server option to all jobsub commands.
-   2016-07-18 Herbert Greenlee : Add back missing project\_utilities import.
-   2016-07-18 Herbert Greenlee : Replace use of /tmp with tempfile.mkdtemp().

larutils v1\_06\_06
------------------------------------------

-   2016-07-19 Lynn Garren : Merge branch ‘release/v05\_15\_01’
-   2016-07-19 Lynn Garren : larutils v1\_06\_06
-   2016-07-19 Lynn Garren : update build
-   2016-07-18 Lynn Garren : add s36:e10