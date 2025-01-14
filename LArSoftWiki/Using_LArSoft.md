

-   [Quick_Links](Quick_Links)
-   [Concepts in LArSoft](https://larsoft.org/important-concepts-in-larsoft/)

# Preliminaries

-   Fermilab computing accounts: see [the process to request access to Fermilab](https://get-connected.fnal.gov/faq/#SABprocess) and [Fermilab computing access](Fermilab_computing_access).
-   See [Load Balanced Access to General Purpose VMs](Load_Balanced_Access_to_General_Purpose_VMs) for information on accessing experiment VMs at Fermilab (e.g., lbnegpvm0X, uboonegpvm0X, etc., collectively known as GPCF.)
-   LArSoft currently supports the platforms listed [here](Supported_platforms). **Users who wish to develop on an unsupported platform may use** [a container approach](Developing_LArSoft_with_Containers).
-   To join the LArSoft mailing list, please follow [these instructions](https://listserv.fnal.gov/users.asp#subscribe_to_list) using the list name LARSOFT.

# Using LArSoft

First-time, or infrequent, users will be well-served to go through the following steps in order:

1.  Start by reading [Concepts in LArSoft](https://larsoft.org/important-concepts-in-larsoft/), the [training material at larsoft.org](https://larsoft.org/training) and other information available at [larsoft.org](https://larsoft.org)
    1.  Also look at your experiment's [Quick Links](Quick_Links) for experiment-specific information.
2.  Choose the correct release from the [List of LArSoft Releases and Release Notes](releases/LArSoft_release_list).
    1.  If you can use a tagged release as is (aside from fcl files which can be modified and used from any directory), you can now run LArSoft.
    2.  If you need to modify the code locally, or use code not yet in a tagged release, then additional steps (below) are required.
3.  Create a working area. This is described in the presentation from the 2019 workshop session on [LArSoft technical details](https://indico.fnal.gov/event/20453/session/5/contribution/2/material/slides/0.pdf).
    1.  To find out which repositories contain the code you need to modify for your task, examine the [List of repositories and their relationships](LArSoft_repositories_packages_and_dependencies).
    2.  If you have questions, ask the relevant code authors and [offline leads](Offlineleads) and [release managers](/LArSoftWiki/LArSoftInternals/Informal_list_of_experiment_contacts).
4.  To modify the code, clone the reference software into your working area from the [LArSoft github](https://github.com/LArSoft) repositories.
    1.  This is where to find [Experiment-specific code](Experiment-specific_code).
    2.  And this is the [Sub-package locations](Sub-package_locations) (e.g., in which repository can I find the `HitFinder` sub-package?)
    3.  See the [Developing With LArSoft](Developing_With_LArSoft) page for more details and guidelines on how to modify or develop new code for LArSoft.
5.  To install a local copy of the pre-built products, or to build and install a local copy of the products for the core LArSoft suite, follow the [Installation Procedures on the Getting LArSoft page](Getting_LArSoft).
    1.  To use cvmfs to access the binaries and header files in a tagged release (thereby avoiding the need to install or build a local copy), follow the [LArSoft cvmfs page](LArSoft_cvmfs_page) instructions.
    2.  Sometimes your local code will fail to build against a new LArSoft release because there are “breaking changes” in the release, which are modifications that require adaptations to the code that references that modified code. These changes and the corrective actions needed are documented on the [Breaking_Changes](releases/Breaking_Changes) page.
    3.  Comments in the code are incorporated into documentation at [LArSoft Doxygen](https://code-doc.larsoft.org/docs/latest/html/index.html) using [the Doxygen tool.](https://www.doxygen.nl/helpers.html)
6.  Recommended.
    1.  Install and run [Igprof profiler](Igprof_profiler).

## Information on GitHub and pull request testing

Start by reviewing the information on [the overview page for using LArSoft with GitHub](Working_with_GitHub). The GitHub repositories are available. Contact your experiment offline management to identify acting Level 2 managers. Send any comments to The Scisoft Team, or via Redmine issues.

## Some hints

-   [Rerun part or all a job on an output file of that job](Rerun_part_of_all_a_job_on_an_output_file_of_that_job).
-   Tips on [Interactive GPVM sessions with terminal multiplexers](Interactive_GPVM_sessions_with_terminal_multiplexers)
-   [Reproducing jobs using the same random number sequences](Reproducing_jobs_using_the_same_random_number_sequences)
-   [Rerunning a job starting from its output](Rerunning_a_job_starting_from_its_output)
-   About [fast cloning](Fast_cloning)
-   [Working with GitHub](Working_with_GitHub) for LArSoft 


# Documentation

-   Description of [Event Displays](Event_Displays) options with links to further information.
-   Description of [The user environment](The_user_environment) with examples.
-   Description of [The developer environment](The_developer_environment) with a picture.
-   Using Geant4 with LArSoft
   
       LArSoft interfaces to Geant4 via the tools provided in the [larg4 repository](https://github.com/LArSoft/larg4), which are built on top of [artg4tk](https://cdcvs.fnal.gov/redmine/projects/artg4tk/wiki/Artg4tk), the more general interface between Geant4 and art. Two modules, larg4Main and larg4SingleGen, are available in larg4 to allow simulation or particles from arbitrary MCTruth collections in the event (and therefore from arbitrary event generators), and a list of particles specified in a FHiCL file, respectively.
    
    A legacy (and now deprecated) interface to Geant4 exists within the larsim/LegacyLArG4 area. Some detectors still use this  “legacy-LArG4” interface. Information on migrating from legacy-LArG4 to the re-factored larg4 can be found on the  [larg4 wiki](https://cdcvs.fnal.gov/redmine/projects/larg4/wiki) page.
    
    Important information about the requirements for GDML files used by the re-factored larg4 can also be found on the  [larg4 wiki](https://cdcvs.fnal.gov/redmine/projects/larg4/wiki). 


## Using HPC with LArSoft

-   Using GPU as a service to accelerate machine learning inference applications.
    -   [ Part One: Overview and introduction to the NuSonic Triton client library ](GPU_as_a_Service)
    -   [Part Two: Setting up the model on the Triton inference server](GPU_as_a_Service_part_two)
    -   [Part Three: Testing the Triton client and model configuration with an inference server](GPU_as_a_Service_part_three)

## Machine Learning in LArSoft

- [NuGraph2 GNN event reconstruction integration](https://larsoft.github.io/LArSoftWiki/NuGraph2_integration)
- [CVN-based neutrino classification using CVN Integration in LArSoft](https://larsoft.github.io/LArSoftWiki/CVN_integration)
- [Waveform region-of-interest finding for supernova event triggering integration](https://larsoft.github.io/LArSoftWiki/Using_raw_waveform)

# How-to

-   [ Getting started with an analysis task: an example ](AnalysisExample)
-   [Running Jobs](Running_Jobs)
