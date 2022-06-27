# CBTTape-File001

## Git Information
<details closed><summary>Click to Expand (or Close)</summary>

### Background
```
This CBTTAPE File was converted from the CBTTAPE distribution format
so that it could be mirrored for access using GitHub. This is a partially
automated process with some manual adjustments as required by each
individual CBT file.

The CBTTAPE file is distributed as a ZIP file that contains, typically,
an XMIT file. This XMIT file must then be received using TSO RECEIVE to
create a PDS that contains the contents of the CBTTAPE file. Some of the
PDS members are also in the XMIT format.

The 'mirror' process performed the following after the PDS was created:

Automated:
  1. Copied the original PDS into a PDS using the Git HLQ
  2. The @FILEnnn, or @FILnnnnn, members were copied into a
     README.md OMVS file.
     - if the file is not found then the information if copied from
       the CBT File 001 section describing the file.
  3. Any members with PDF, PPT, ZIP, DOCX, etc. were copied into
     individual datasets. Some will be moved to an OMVS file with
     a more meaningful file name based on a CBT File specific
     converstion control data.
  4. Any members in XMIT format were processed using TSO RECEIVE into
     datasets under the Git HLQ, using the member name as a qualifier.
  5. Any members with (4) in XMIT format were also processed using TSO
     RECEIVE.
  6. All members that were copied out to individual datasets were
     deleted, including the XMIT members.

Manual (using ZIGI):
  1. The Git repository was created on GitHub without adding any files
     so that it is empty on GitHub for now.
  2. ZIGI was used to create the repository by adding the datasets
     under the Git HLQ to the repository.
  3. The ZIGI repository is updated with the GitHub SSH Git URL (1)

Manual (under OMVS):
  1. PDF, PPT, ZIP, etc. were renamed to more meaningful file names with
     an appropriate suffix in lower case.
     - unless this was automated using a CBT File specific control file

Manual (using ZIGI):
  1. ZIGI now performs the Git Add, Commit, and Push to the GitHub
     repository.
```
### Copying the Git files into z/OS Datasets

```
The Git repository was then created using ZIGI, the z/OS ISPF Git
Interface, which can be found at https://zigi.rocks and which uses the
z/OS OMVS port of Git provided by Rocket software.

**Note:** If you performed a git clone from OMVS without using ZIGI then
you can use the zginstall.rex to 'upload' the files to z/OS, creating
the z/OS datasets. See zginstall.readme for more information on it.

When using the zginstall.rex tool the last thing it does is inform the
user of a z/OS REXX to invoke to add the ISPF statistics to the z/OS
partitioned dataset members. This is something that ZIGI does
automatically.

```

### Installation Information
```
Because of this process, any installation documentation or automation
provided with the file may not work as provided and may require some
adjustments.

```

</details>

## CBT File Information

```

--------------------------------------------------------------------------------
//***FILE 001 IS THE JCL THAT CREATED THIS TAPE (YOU ARE            *   FILE 001
//*           READING IT NOW).  The REAL JCL is on File 008.        *   FILE 001
//*                                                                 *   FILE 001
//*           Please see the assembler program called CBTUPD        *   FILE 001
//*           that is on File 004 and on File 006.  This program    *   FILE 001
//*           will introduce ./ ADD NAME= cards into this file,     *   FILE 001
//*           so that it can be conveniently broken up into         *   FILE 001
//*           members of a partitioned dataset, and it may be       *   FILE 001
//*           read in more "bite-sized" pieces.                     *   FILE 001
//*                                                                 *   FILE 001
//*           There are also some more tools for handling this      *   FILE 001
//*           documentation, which may be found on File 006.        *   FILE 001
//*                                                                 *   FILE 001
//*           Some ancient remarks from Arnie Casinghino:           *   FILE 001
//*           (They still may be relevant.)                         *   FILE 001
//*                                                                 *   FILE 001
//*                            SUNGARD                              *   FILE 001
//*                                                                 *   FILE 001
//*           THE FOLLOWING IS A COMMENT FROM MR ARTHUR TANSKY      *   FILE 001
//*           OF SUNGARD IN VOORHEES, NEW JERSEY. IT MAY BE TO      *   FILE 001
//*           YOUR ADVANTAGE TO FOLLOW HIS ADVICE.                  *   FILE 001
//*                                                                 *   FILE 001
//*           TO KEEP FILE 001 FROM TAKING UP SO MUCH ROOM, YOU     *   FILE 001
//*           CAN EDIT OUT CERTAIN OF THE BEGINNING LINES WHICH     *   FILE 001
//*           ARE SELDOM USED (SUCH AS THE ADDRESS).  BUT THIS      *   FILE 001
//*           DOES NOT SAVE TOO MUCH.  THE REAL SAVINGS COMES       *   FILE 001
//*           WHEN YOU GET RID OF THE //* AT THE BEGINNING OF       *   FILE 001
//*           EACH LINE AND ESPECIALLY THE * AT THE END OF EACH     *   FILE 001
//*           LINE.  YOU CAN USE SPF TO COPY THE DATASET TO A VB    *   FILE 001
//*           FILE.  THE FILE TAKES UP 34  3380 TRACKS (BLOCKED     *   FILE 001
//*           AT 9040) IN FIXED FORMAT AND ONLY 20 TRACKS VB AT     *   FILE 001
//*           9076.  THIS SAVINGS OF 14 TRACKS ALSO TRANSLATES      *   FILE 001
//*           TO CPU-TIME AND REAL-TIME WHEN SEARCHING THE FILE,    *   FILE 001
//*           IN THAT THERE ARE THAT MANY LESS BYTES TO SEARCH.     *   FILE 001
//*           MR TANSKY'S CALCULATIONS SHOW A 40% SAVINGS.          *   FILE 001
//*                                                                 *   FILE 001
//*           WE, HOWEVER, WILL NOT CHANGE THE FILE, SINCE          *   FILE 001
//*           FILE 001 IS USED AS INPUT TO FILE 042 OF THIS         *   FILE 001
//*           TAPE, WHICH IS USED TO CREATE THE INPUT TO AN         *   FILE 001
//*           INFOMVS DATA BASE.                                    *   FILE 001
//*                                                                 *   FILE 001
```
