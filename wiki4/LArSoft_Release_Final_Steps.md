LArSoft Release Final Steps[¶](#LArSoft-Release-Final-Steps)
============================================================

-   **Table of contents**
-   [LArSoft Release Final Steps](#LArSoft-Release-Final-Steps)
    -   [Make the cross package tag](#Make-the-cross-package-tag)
    -   [Update the release notes](#Update-the-release-notes)
    -   [Update doxygen](#Update-doxygen)
    -   [Merge the changes with develop](#Merge-the-changes-with-develop)
    -   [Announcing the release](#Announcing-the-release)


Make the cross package tag[¶](#Make-the-cross-package-tag)
----------------------------------------------------------

-   This step can only be done by someone with manager privileges for all the larsoft repositories.
    -   setup laradmin
    -   cp-lar-tag vxx\_yy\_zz \<larsoftobj version\>
    -   This will apply the tag LARSOFT\_SUITE\_vxx\_yy\_zz to the appropriate tag that was used to build vxx\_yy\_zz in the various larsoft repositories.
-   The cross package tag must be added by hand for **larutils** and **larbatch**
    -   cd \$MRB\_SOURCE/\<larbatch|larutils\>
    -   git checkout master
    -   git diff \<new tag for this package\>
    -   If there are differences the cross package tag cannot be added
    -   git tag -a -m“LARSOFT\_SUITE\_vxx\_yy\_zz” LARSOFT\_SUITE\_vxx\_yy\_zz
    -   git push –tags


Update the release notes[¶](#Update-the-release-notes)
------------------------------------------------------

-   run make-release-notes (found in laradmin)

-   make-release-notes \<working\_directory\> \<new tag\> \<old tag\>

-   the script will create a \<new tag\> subdirectory under \<working\_directory\>, checkout the larsoft suite there, and run git log
-   note that make-release-notes uses the cross package tag

-   the first line in ReleaseNotes-\<version\> is the entry for the [Release Notes table](LArSoft_release_list)
-   the remainder of the file is used to populate the release note itself


Update doxygen[¶](#Update-doxygen)
----------------------------------

-   ssh -l larsoft uboonegpvm02.fnal.gov
-   cd doxygen
-   ./update\_lar\_doxygen.sh \>& update.log


Merge the changes with develop[¶](#Merge-the-changes-with-develop)
------------------------------------------------------------------

-   Notice that we need to make sure that the new release is available before we update the develop branch with new version numbers.
-   This step should be done in \$MRB\_SOURCE
-   tagLAr merge vxx\_yy\_zz
    -   tagLAr will merge local branch release/vxx\_yy\_zz with the head of develop
    -   if conflicts occur, the merge must be done by hand for each repository


            cd $MRB_SOURCE/larpackage
            git checkout develop
            git pull
            git merge release/vxx_yy_zz
            (resolve conflicts)
            git push origin develop

-   Once this step is complete, it is safe to remove the working directory for this release.


Announcing the release[¶](#Announcing-the-release)
--------------------------------------------------

-   Send email announcing that the release is built and available
    -   Make sure you include a link to the release notes.
    -   Mention the purpose of the release and any feature branches needed by the experiments.
    -   Also include a link to the download page and list the platforms for which the binary distribution is available.