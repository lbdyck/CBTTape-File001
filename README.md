# CBTTape-File001
```
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
