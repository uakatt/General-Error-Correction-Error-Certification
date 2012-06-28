General Error Correction Error Certification
======================

This git repository represents the University of Arizona (the UA)'s _General Error Correction Error Certification_ modification to **KFS 3.0**, in the form of patch files (generated by svn diff), liquibase scripts, and documentation.
This "patch package" is designed to be informative to technical developers in the position to
apply patch files to the java source code of KFS. In order to better serve such an endeavor,
this README contains several informative sections:

* <a href="#jiras">List of Jiras</a> - This list contains every Jira ticket at the University of Arizona
  that relates to this modification. It provides reverse documentation back to the developers at
  the UA in case of questions regarding how this patch package was created.
* <a href="#liquibase-changesets">List of Liquibase Changesets</a> - This list contains any
  liquibase changeset files that were associated with this modification.
* <a href="#patch-files">List of Patch Files</a> - This is a list of each patch file that needs
  to be applied to the KFS source code in order to realize the modification. This list does _not_
  include patch files for revisions that didn't touch the `trunk/` at the UA.
  Before a modification was merged with `trunk/`, it may have been tweaked, reworked, refactored,
  code reviewed, etc, in handfuls of revisions in a feature branch.
* <a href="#revisions">List of Revisions</a> - This list contains every revision associated with
  this modification. Many of which, as you will see, only touch files in a feature branch. The
  revisions that actually made it into the actual modification touch files in `trunk/`. The list
  of patch files is a better reference of which are these revisions.
* <a href="#files">Lists of Files</a> - These lists contain every file that was created,
  modified, or deleted for this enhancement.
* <a href="#post-mod-changes">List of Post-Modification Changes</a> - This list contains
  revision numbers that are _not_ included in the patches, or raw patches, but that touched one
  or more key files involved in this modification.

<h2>Jiras</h2>

This is a list of Jira tickets at the University of Arizona that relate to this modification. The subversion revisions tagged against each such jira are also listed:

* **KITT-353**: (The main jira for this modification)<br />
  revisions: #2142, #2143, #2144, #2145, #2146, #2147, #2148, #2998, #2999, #3003, #3004, #3005, #3006, #3007, #3008, #3009, #3010, #3011, #3012, #3014, #3015, #3016, #3017, #3018, #3019, #3020, #3022, #3025, #3143, #3144, #3145, #3146, #3147, #3148, #4027, #4210, #4607, #4688, #4753, #5240, #6860, #6861, #6862, #6863, #6864, #6865, #7228, #7229, #7232, #7233, #7238, #7240, #7241
* **KITT-744**: (Parameters needed for this modification)<br />
  revisions: #7270, #7272
* **KITT-2004**: (A change request against this modification)<br />
  revisions: #15345

<h2>Liquibase Changesets</h2>

* `latest/dat/KRNS_PARM_T.xml` saw the following activity:
  * changed in #7270 (resultant file: [`whole_files/r7270/KRNS_PARM_T.xml`](General-Error-Correction-Error-Certification/blob/master/whole_files/r7270/KRNS_PARM_T.xml)).
* `update/KITT-744.xml` saw the following activity:
  * created in #7270 (resultant file: [`whole_files/r7270/KITT-744.xml`](General-Error-Correction-Error-Certification/blob/master/whole_files/r7270/KITT-744.xml)).

(2 changes among 2 files)

<h2>Patch Files</h2>

This is a list of all of the patches for revisions that affected files in `trunk/`. The filenames in each has been modified, for easy digestion. UA's subversion server manages many Kuali projects in one Subversion project, so a file path like:

```
financial-system/kfs/trunk/src/org/kuali/kfs...
```

has been modified to:

```
src/org/kuali/kfs...
```

* [`patches/02142_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/02142_KITT-353_cleaned.diff) is the patch file for #2142.
* [`patches/02143_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/02143_KITT-353_cleaned.diff) is the patch file for #2143.
* [`patches/02144_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/02144_KITT-353_cleaned.diff) is the patch file for #2144.
* [`patches/02145_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/02145_KITT-353_cleaned.diff) is the patch file for #2145.
* [`patches/02146_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/02146_KITT-353_cleaned.diff) is the patch file for #2146.
* [`patches/02147_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/02147_KITT-353_cleaned.diff) is the patch file for #2147.
* [`patches/02148_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/02148_KITT-353_cleaned.diff) is the patch file for #2148.
* [`patches/02998_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/02998_KITT-353_cleaned.diff) is the patch file for #2998.
* [`patches/02999_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/02999_KITT-353_cleaned.diff) is the patch file for #2999.
* [`patches/03003_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/03003_KITT-353_cleaned.diff) is the patch file for #3003.
* [`patches/03004_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/03004_KITT-353_cleaned.diff) is the patch file for #3004.
* [`patches/03005_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/03005_KITT-353_cleaned.diff) is the patch file for #3005.
* [`patches/03006_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/03006_KITT-353_cleaned.diff) is the patch file for #3006.
* [`patches/03007_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/03007_KITT-353_cleaned.diff) is the patch file for #3007.
* [`patches/03008_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/03008_KITT-353_cleaned.diff) is the patch file for #3008.
* [`patches/03009_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/03009_KITT-353_cleaned.diff) is the patch file for #3009.
* [`patches/03010_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/03010_KITT-353_cleaned.diff) is the patch file for #3010.
* [`patches/03011_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/03011_KITT-353_cleaned.diff) is the patch file for #3011.
* [`patches/03012_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/03012_KITT-353_cleaned.diff) is the patch file for #3012.
* [`patches/03014_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/03014_KITT-353_cleaned.diff) is the patch file for #3014.
* [`patches/03015_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/03015_KITT-353_cleaned.diff) is the patch file for #3015.
* [`patches/03016_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/03016_KITT-353_cleaned.diff) is the patch file for #3016.
* [`patches/03017_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/03017_KITT-353_cleaned.diff) is the patch file for #3017.
* [`patches/03018_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/03018_KITT-353_cleaned.diff) is the patch file for #3018.
* [`patches/03019_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/03019_KITT-353_cleaned.diff) is the patch file for #3019.
* [`patches/03020_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/03020_KITT-353_cleaned.diff) is the patch file for #3020.
* [`patches/03022_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/03022_KITT-353_cleaned.diff) is the patch file for #3022.
* [`patches/03025_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/03025_KITT-353_cleaned.diff) is the patch file for #3025.
* [`patches/03143_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/03143_KITT-353_cleaned.diff) is the patch file for #3143.
* [`patches/03144_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/03144_KITT-353_cleaned.diff) is the patch file for #3144.
* [`patches/03145_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/03145_KITT-353_cleaned.diff) is the patch file for #3145.
* [`patches/03146_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/03146_KITT-353_cleaned.diff) is the patch file for #3146.
* [`patches/03147_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/03147_KITT-353_cleaned.diff) is the patch file for #3147.
* [`patches/03148_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/03148_KITT-353_cleaned.diff) is the patch file for #3148.
* [`patches/04027_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/04027_KITT-353_cleaned.diff) is the patch file for #4027.
* [`patches/04210_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/04210_KITT-353_cleaned.diff) is the patch file for #4210.
* [`patches/04607_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/04607_KITT-353_cleaned.diff) is the patch file for #4607.
* [`patches/04688_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/04688_KITT-353_cleaned.diff) is the patch file for #4688.
* [`patches/04753_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/04753_KITT-353_cleaned.diff) is the patch file for #4753.
* [`patches/05240_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/05240_KITT-353_cleaned.diff) is the patch file for #5240.
* [`patches/06860_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/06860_KITT-353_cleaned.diff) is the patch file for #6860.
* [`patches/06861_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/06861_KITT-353_cleaned.diff) is the patch file for #6861.
* [`patches/06862_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/06862_KITT-353_cleaned.diff) is the patch file for #6862.
* [`patches/06863_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/06863_KITT-353_cleaned.diff) is the patch file for #6863.
* [`patches/06864_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/06864_KITT-353_cleaned.diff) is the patch file for #6864.
* [`patches/06865_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/06865_KITT-353_cleaned.diff) is the patch file for #6865.
* [`patches/07228_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/07228_KITT-353_cleaned.diff) is the patch file for #7228.
* [`patches/07229_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/07229_KITT-353_cleaned.diff) is the patch file for #7229.
* [`patches/07232_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/07232_KITT-353_cleaned.diff) is the patch file for #7232.
* [`patches/07233_KITT-353_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/07233_KITT-353_cleaned.diff) is the patch file for #7233.
* [`patches/15345_KITT-2004_cleaned.diff`](General-Error-Correction-Error-Certification/blob/master/patches/15345_KITT-2004_cleaned.diff) is the patch file for #15345.

<h2>Revisions</h2>

This is an ordered list of revisions that relate to this modification. There may not be a patch
file for every revision listed below for the following reasons:

* A revision might only affect a branch, perhaps one where development primarily took place. Any
  changes that finally made it into `trunk/` will be seen in revisions that specifically touch
  files in `trunk/`. Therefore, we do not create patch files for revisions that only affect a
  branch.
* A revision might only include a liquibase changeset that is executed by some automated process.
  Since each institution maintains different revision controls on their database, liquibase
  changesets are not provided as patches. They are instead presented as intact files under the
  `liquibase-changesets/` directory.

[Here](General-Error-Correction-Error-Certification/blob/master/patch_log.txt) is a printout of `svn log -v` for each revision.

*   \#2142 was committed against KITT-353 on 2009-05-27 00:50:20 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#2143 was committed against KITT-353 on 2009-05-27 00:50:55 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#2144 was committed against KITT-353 on 2009-05-27 00:51:11 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#2145 was committed against KITT-353 on 2009-05-27 00:53:31 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#2146 was committed against KITT-353 on 2009-05-27 00:53:46 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#2147 was committed against KITT-353 on 2009-05-27 00:54:04 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#2148 was committed against KITT-353 on 2009-05-27 00:54:29 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#2998 was committed against KITT-353 on 2009-06-16 18:57:58 UTC by <strong>hlo</strong>.

    > KITT-353 Adding Error Certification table
*   \#2999 was committed against KITT-353 on 2009-06-16 19:00:40 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#3003 was committed against KITT-353 on 2009-06-16 20:51:57 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#3004 was committed against KITT-353 on 2009-06-16 20:53:55 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#3005 was committed against KITT-353 on 2009-06-16 20:54:07 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#3006 was committed against KITT-353 on 2009-06-16 20:54:36 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#3007 was committed against KITT-353 on 2009-06-16 20:58:08 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#3008 was committed against KITT-353 on 2009-06-16 20:58:39 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#3009 was committed against KITT-353 on 2009-06-16 21:00:52 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#3010 was committed against KITT-353 on 2009-06-16 21:01:55 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#3011 was committed against KITT-353 on 2009-06-16 21:02:12 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#3012 was committed against KITT-353 on 2009-06-16 21:02:24 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#3014 was committed against KITT-353 on 2009-06-16 21:03:34 UTC by <strong>hlo</strong>.

    > KITT-353 Adding Error Certification
*   \#3015 was committed against KITT-353 on 2009-06-16 21:05:09 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#3016 was committed against KITT-353 on 2009-06-16 21:05:49 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#3017 was committed against KITT-353 on 2009-06-16 21:07:23 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#3018 was committed against KITT-353 on 2009-06-16 21:08:48 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#3019 was committed against KITT-353 on 2009-06-16 21:10:24 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#3020 was committed against KITT-353 on 2009-06-16 21:13:48 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#3022 was committed against KITT-353 on 2009-06-16 21:16:29 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#3025 was committed against KITT-353 on 2009-06-16 21:33:09 UTC by <strong>hlo</strong>.

    > KITT-353 Modified LOG lines.
*   \#3143 was committed against KITT-353 on 2009-06-22 23:31:39 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#3144 was committed against KITT-353 on 2009-06-22 23:31:53 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#3145 was committed against KITT-353 on 2009-06-22 23:32:29 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#3146 was committed against KITT-353 on 2009-06-22 23:32:50 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#3147 was committed against KITT-353 on 2009-06-22 23:33:25 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#3148 was committed against KITT-353 on 2009-06-22 23:39:27 UTC by <strong>hlo</strong>.

    > KITT-353 Adding UA version of GEC Form.
*   \#4027 was committed against KITT-353 on 2009-07-21 20:40:13 UTC by <strong>hlo</strong>.

    > KITT-353 Changed parent reference to the rSmart bean.
*   \#4210 was committed against KITT-353 on 2009-07-31 19:09:45 UTC by <strong>hlo</strong>.

    > KITT-353 Changing bean name back to GeneralErrorCorrectionDocument.
*   \#4607 was committed against KITT-353 on 2009-08-31 17:20:41 UTC by <strong>hlo</strong>.

    > KITT-353  Fixing typos in comments.
*   \#4688 was committed against KITT-353 on 2009-09-05 01:23:32 UTC by <strong>hlo</strong>.

    > KITT-353 Cleaned up code.
*   \#4753 was committed against KITT-353 on 2009-09-08 21:21:47 UTC by <strong>hlo</strong>.

    > KITT-353 Refactored code.
*   \#5240 was committed against KITT-353 on 2009-10-02 21:41:20 UTC by <strong>hlo</strong>.

    > KITT-353 KITT-360 Re-adding previous code changes.
*   \#6860 was committed against KITT-353 on 2010-01-06 21:24:17 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#6861 was committed against KITT-353 on 2010-01-06 21:24:51 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#6862 was committed against KITT-353 on 2010-01-06 21:26:27 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#6863 was committed against KITT-353 on 2010-01-06 21:26:47 UTC by <strong>hlo</strong>.

    > KITT-353
*   \#6864 was committed against KITT-353 on 2010-01-06 21:28:12 UTC by <strong>hlo</strong>.

    > KITT-353, KITT-360 Adding parms for YEGE. Also adding back parms for YEST.
*   \#6865 was committed against KITT-353 on 2010-01-06 21:30:31 UTC by <strong>hlo</strong>.

    > KITT-353 Adding YEGE.
*   \#7228 was committed against KITT-353 on 2010-01-20 18:17:57 UTC by <strong>hlo</strong>.

    > KITT-353 Fixed parameter error - wasn't reading correct parameter for YEGE.
*   \#7229 was committed against KITT-353 on 2010-01-20 18:20:37 UTC by <strong>hlo</strong>.

    > KITT-353 Removed because this class is unnecessary.
*   \#7232 was committed against KITT-353 on 2010-01-20 18:24:08 UTC by <strong>hlo</strong>.

    > KITT-353, KITT-360 Modified because edu/arizona versions of GEC and SET forms removed.
*   \#7233 was committed against KITT-353 on 2010-01-20 18:25:38 UTC by <strong>hlo</strong>.

    > KITT-353, KITT-360 Re-adding YEST and YEGE parms.
*   \#15345 was committed against KITT-2004 on 2010-12-23 00:20:08 UTC by <strong>hlo@CATNET.ARIZONA.EDU</strong>.

    > KFSI-2900
    > KITT-2004
    > Adding reference origin code to validations and unit test. Also modified error message.

<h2>Files</h2>

Files **created** for this modification (20 files)

    /work/src/edu/arizona/kfs/fp/businessobject/ErrorCertification.java
    /work/src/edu/arizona/kfs/fp/businessobject/datadictionary/ErrorCertification.xml
    /work/src/edu/arizona/kfs/fp/document/GeneralErrorCorrectionDocument.java
    /work/src/edu/arizona/kfs/fp/document/YearEndGeneralErrorCorrectionDocument.java
    /work/src/edu/arizona/kfs/fp/document/datadictionary/GeneralErrorCorrectionDocument.xml
    /work/src/edu/arizona/kfs/fp/document/datadictionary/YearEndGeneralErrorCorrectionDocument.xml
    /work/src/edu/arizona/kfs/fp/document/validation/configuration
    /work/src/edu/arizona/kfs/fp/document/validation/configuration/FinancialProcessingValidators.xml
    /work/src/edu/arizona/kfs/fp/document/validation/configuration/GeneralErrorCorrectionValidation.xml
    /work/src/edu/arizona/kfs/fp/document/validation/impl/EntryNotFoundException.java
    /work/src/edu/arizona/kfs/fp/document/validation/impl/ErrorCertificationValidation.java
    /work/src/edu/arizona/kfs/fp/document/validation/impl/GeneralErrorCorrectionDocumentPreRules.java
    /work/src/edu/arizona/kfs/fp/document/validation/impl/GeneralErrorCorrectionErrorCertificationValidation.java
    /work/src/edu/arizona/kfs/fp/document/validation/impl/GeneralErrorCorrectionRefNumberValidation.java
    /work/src/edu/arizona/kfs/fp/document/web
    /work/src/edu/arizona/kfs/fp/document/web/struts
    /work/src/edu/arizona/kfs/fp/document/web/struts/GeneralErrorCorrectionForm.java
    /work/src/edu/arizona/kfs/fp/document/web/struts/YearEndGeneralErrorCorrectionForm.java
    /work/src/edu/arizona/kfs/sys/KFSConstants.java
    /work/web-root/WEB-INF/tags/fp/errorCertification.tag

Files **modified** for this modification (11 files)

    /test/unit/src/edu/arizona/kfs/fp/document/validation/GECErrorCertificationValidationTest.java
    /work/db/scripts/arizona/data.sql
    /work/db/scripts/arizona/schema-oracle.sql
    /work/src/arizona-ApplicationResources.properties
    /work/src/edu/arizona/kfs/fp/ojb-fp.xml
    /work/src/edu/arizona/kfs/fp/spring-fp.xml
    /work/src/edu/arizona/kfs/sys/AZKFSConstants.java
    /work/src/edu/arizona/kfs/sys/KFSKeyConstants.java
    /work/web-root/WEB-INF/struts-config.xml
    /work/web-root/jsp/fp/GeneralErrorCorrection.jsp
    /work/web-root/jsp/fp/YearEndGeneralErrorCorrection.jsp

<h2>Post Mod Changes</h2>

For each file that was changed or added for this modification, I've looked at its history in subversion (`svn log <file_name>`) to find whether later fixes were committed against this modification that I might have missed. There were some :) They may be fixes to the modification, or further enhancements, or changes completely unrelated. Please contact the UA for more information about a given revision number, or Jira ticket. Here they are:

*   **#4353** touches `/work/web-root/jsp/fp/GeneralErrorCorrection.jsp`.

    > Merging build-1233
*   **#4397** touches: 
    * `/work/web-root/WEB-INF/tags/fp/errorCertification.tag`
    * `/work/web-root/jsp/fp/GeneralErrorCorrection.jsp`

    > Adding back error certification mod
*   **#4897** touches: 
    * `/work/src/edu/arizona/kfs/fp/document/validation/configuration/GeneralErrorCorrectionValidation.xml`
    * `/work/src/edu/arizona/kfs/fp/document/validation/impl/GeneralErrorCorrectionRefNumberValidation.java`
    * `/work/src/edu/arizona/kfs/fp/document/GeneralErrorCorrectionDocument.java`
    * `/work/src/edu/arizona/kfs/fp/document/validation/impl/EntryNotFoundException.java`
    * `/work/src/edu/arizona/kfs/fp/document/validation/impl/ErrorCertificationValidation.java`
    * `/work/src/edu/arizona/kfs/fp/document/validation/impl/GeneralErrorCorrectionErrorCertificationValidation.java`
    * `/work/src/edu/arizona/kfs/fp/document/datadictionary/GeneralErrorCorrectionDocument.xml`
    * `/work/src/edu/arizona/kfs/fp/businessobject/ErrorCertification.java`
    * `/work/src/edu/arizona/kfs/fp/businessobject/datadictionary/ErrorCertification.xml`
    * `/work/src/edu/arizona/kfs/fp/document/validation/impl/GeneralErrorCorrectionDocumentPreRules.java`

    > Readding modifications
*   **#5534** touches `/work/web-root/jsp/fp/GeneralErrorCorrection.jsp`.

    > merging 1310
*   **#5543** touches `/work/src/edu/arizona/kfs/fp/document/datadictionary/GeneralErrorCorrectionDocument.xml`.

    > KITT-405 Adding object sub type code routing.
*   **#10490** touches `/work/src/edu/arizona/kfs/fp/document/validation/configuration/GeneralErrorCorrectionValidation.xml`.

    > Merging KITT-803.
*   **#12343** touches `/work/src/edu/arizona/kfs/fp/document/YearEndGeneralErrorCorrectionDocument.java`.

    > KFSI-2284: break the YEGE for the sake of testing (have it do extra search attribute indexing)
*   **#12428** touches `/work/src/edu/arizona/kfs/fp/document/YearEndGeneralErrorCorrectionDocument.java`.

    > KITT-1526: roll back extra search attribute indexing on YEGE
*   **#15500** touches `/work/src/edu/arizona/kfs/fp/document/validation/impl/GeneralErrorCorrectionDocumentPreRules.java`.

    > KFSI-2941
    > KITT-2048
    > Fixed logic in PDCO files so that accounting line will get imported. Created new arizona PDCO document and modify corresponding imports to match.

*   **#17111** touches `/work/src/edu/arizona/kfs/fp/document/validation/configuration/GeneralErrorCorrectionValidation.xml`.

    > KFSI-2421
    > KITT-1934
    > First commit of GTE to trunk
*   **#24304** touches `/work/src/edu/arizona/kfs/fp/document/YearEndGeneralErrorCorrectionDocument.java`.

    > KFSI-6180
    > KATTS-32
    > Pulled over methods from org version of YearEndGeneralErrorCorrection.java because of inheritance and edu override.
*   **#24805** touches `/work/src/edu/arizona/kfs/fp/document/GeneralErrorCorrectionDocument.java`.

    > KFSI-6427 KITT-3085 make sure that the new copy gets its own certification table to prevent overwriting

(12 revisions)

The following files were ignored here:

    struts-config.xml
    arizona-ApplicationResources.properties
    data.sql
    schema-oracle.sql
    spring-fp.xml
    AZKFSConstants.java
    KFSKeyConstants.java
    ojb-fp.xml
    KFSConstants.java
    FinancialProcessingValidators.xml

This means, for example, that `struts-config.xml` was changed for this modification, but `struts-config.xml`'s history was not used to build this list of revisions.

