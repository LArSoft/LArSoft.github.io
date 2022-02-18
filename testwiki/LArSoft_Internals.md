# LArSoft Internals



## LArSoft code management and distribution

-   [Adding / removing users](Adding_/_removing_users)
-   Administrative scripts will be kept in the larreltools repository.
-   [LArSoft release management](LArSoft_release_management)
    -   [How to tag and build a normal LArSoft vxx_yy_zz release](How_to_tag_and_build_a_LArSoft_vx_yy_zz_release)
    -   [How to tag and build a LArSoft patch release](How_to_tag_and_build_a_LArSoft_patch_release)
    -   [Installing products on cvmfs](Installing_products_on_cvmfs)
-   [Informal list of experiment contacts](Informal_list_of_experiment_contacts)
-   [Policy for development from a tagged release](Policy_for_development_from_a_tagged_release)
-   [Procedure to create a new version of larsoft_data, uboone_data, etc.](Procedure to create a new version of larsoft_data)
-   [Installation procedures](Installation_procedures)
-   [LArSoft cvmfs](LArSoft_cvmfs)

## Repository cleanup

-   [Removing old feature branches](Removing_old_feature_branches)
-   [Removing old history](Removing_old_history)
-   [Truncating commit history](Truncating_commit_history)

## who does what

[What Lynn does](What_Lynn_does)

## Pages to update and move

Some pages in LArSoft have a combination of useful and out-of-date information. It would be good to at least remove the out-of-date material, even better would be to update it. The following is a list. Feel free to revise any of the pages and suggest where they should go. (Note, some information may belong partly on larsoft.org and partly in redmine.)

-   [OBSOLETE Using LArSoft on the GPVM nodes](OBSOLETE_Using_LArSoft_on_the_GPVM_nodes) - review and update (and place in \[\[Developing with LArSoft\]\] or \[\[Using LArSoft\]\])
-   [Geometry](Geometry) - should this be split between [larsoft.org](http://larsoft.org/important-concepts-in-larsoft/geometry/) and \[\[Developing with LArSoft\]\] could be under Designing, or under Examples.
-   [Reconstruction](Reconstruction) - merge into larsoft.org?
-   [Simulation](Simulation) - update code references, split?
-   [Space Points](Space_Points) - out of date?
-   [larsoftsvn:Seed Finding and Bezier Tracking](https://cdcvs.fnal.gov/redmine/projects/larsoftsvn/wiki/Seed_Finding_and_Bezier_Tracking) - look at legacy info, maybe delete, or find owner?
-   [larsoftsvn:Optical Simulations](https://cdcvs.fnal.gov/redmine/projects/larsoftsvn/wiki/Optical_Simulations) - - look at legacy info, update, split?
-   [dependencies](dependencies)

## [OBSOLETE FNAL Redmine tricks](OBSOLETE_FNAL_Redmine_tricks)

-   replace with github wiki tips?

## Ongoing Projects

[Architecture revision](Architecture_revision)

-   [Data products architecture and design](Data_products_architecture_and_design)
    -   [action items](DataProductsArchitectureActionItems)
-   [Data product revision (phase II)](Data_product_revision_(phase_II))

[Usability improvements](Usability_improvements)

[LArSoft License](LArSoft_License)

## Code cleanup

-   [OBSOLETE Services and modules scheduled for removal](OBSOLETE_Services_and_modules_scheduled_for_removal)

## Completed Projects

[Building with clang](Building_with_clang)  
[Migration to root 6](Migration_to_root_6)

## LArSoft code analysis

-   [Code analysis process](https://cdcvs.fnal.gov/redmine/projects/larsoft/wiki/Code_analysis_process_and_tools)
-   [Code and Performance analysis tools](Code_and_Performance_analysis_tools)
-   [PMA module code analysis](PMA_module_code_analysis)

## Profiling tests

-   [ProtoDUNE and DUNE Far Detector simulation and reconstruction workflows (v06_57_00)](ProtoDUNE_and_DUNE_Far_Detector_simulation_and_reconstruction_workflows_(v06_57_00))

## Legacy Redmine project sites

These were the sites used when LArSoft was developed under cvs and svn + SoftRelTools, respectively:

[ LArSoft-cvs wiki for the legacy cvs-based LArSoft project](https://cdcvs.fnal.gov/redmine/projects/larsoft-cvs/wiki/)  
[ LArSoft-svn wiki for the legacy svn-based LArSoft project](https://cdcvs.fnal.gov/redmine/projects/larsoftsvn/wiki/)

As of Jan 24, 2014, LArSoft transitioned from svn / SRT to git / mrb / ups, but we retain the legacy projects for historical reasons.