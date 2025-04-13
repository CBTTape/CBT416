# CBT416
Converted to GitHub via [cbt2git](https://github.com/wizardofzos/cbt2git)

This is still a work in progress. GitHub repos will be deleted and created during this period...

```
//***FILE 416 IS FROM DELUXE CHECK PRINTERS AND CONTAINS THE        *   FILE 416
//*           FOLLOWING.  THIS FILE IS IN IEBUPDTE SYSIN FORMAT     *   FILE 416
//*           SEE THE MEMBER CALLED $INDEX FOR ADDITIONAL           *   FILE 416
//*           INFORMATION.                                          *   FILE 416
//*                                                                 *   FILE 416
//*    CATLIST   -  THIS PROGRAM WILL DO A VERY FAST LISTING        *   FILE 416
//*                 OF AN ICF CATALOG FOR GENERATION DATASETS       *   FILE 416
//*                 AND NONVSAM DATASETS.  THE LISTING IS IN        *   FILE 416
//*                 THE SAME FORMAT AS IDCAMS (WE USED IT TO        *   FILE 416
//*                 BUILD A TMC) BUT THE OUTPUT FORMAT WOULD        *   FILE 416
//*                 BE EASY TO CHANGE.  THE PROGRAM MUST RUN        *   FILE 416
//*                 AUTHORIZED (AC=1) BECAUSE IT OPENS THE          *   FILE 416
//*                 CATALOG AS A DATASET.  ALSO THERE IS A          *   FILE 416
//*                 MODESET WE USED TO ALLOW US TO BYPASS RACF      *   FILE 416
//*                 CHECKING.  (RACF THINKS YOU NEED ALTER          *   FILE 416
//*                 ACCESS TO READ THE DATASET AND ALL OF OUR       *   FILE 416
//*                 CATALOGS HAVE A UACC OF UPDATE).  ALL THAT      *   FILE 416
//*                 WAS DONE IN KEY ZERO WAS TO SET THE             *   FILE 416
//*                 JSCBPASS BIT ON.  THE SPEED INCREASE OF         *   FILE 416
//*                 THIS PROGRAM WAS SEVERAL ORDERS OF              *   FILE 416
//*                 MAGNITUDE BETTER THAN IDCAMS ON A LARGE         *   FILE 416
//*                 ICF CATALOG.                                    *   FILE 416
//*                                                                 *   FILE 416
//*    CMDLOFF   -  THIS COMMAND WILL ISSUE THE COMMAND PASSED      *   FILE 416
//*                 TO IT AND THEN CAUSE LOGOFF OF THE USER.        *   FILE 416
//*                 THIS IS USEFUL IN THE SITUATION WHERE YOU       *   FILE 416
//*                 WANT A USER TO EXIST IN A PROTECTED             *   FILE 416
//*                 ENVIRONMENT.  EX. CMDLOFF ISPSTART              *   FILE 416
//*                 PANEL(USERSEL)                                  *   FILE 416
//*                                                                 *   FILE 416
//*    DLXAUTHC  -  THIS COMMAND WILL ISSUE THE COMMAND PASSED      *   FILE 416
//*                 TO AFTER SETTING THE JSCBAUTH BIT ON.  WHEN     *   FILE 416
//*                 THE COMMAND COMPLETES THE JSCBAUTH BIT          *   FILE 416
//*                 WILL BE SET OFF.  THE JSCB TAMPERING IS         *   FILE 416
//*                 DONE IN A USER SVC.  YOU MUST REPLACE THE       *   FILE 416
//*                 USERSVC MACRO WITH YOUR OWN INTEGRITY           *   FILE 416
//*                 VIOLATION.  THIS COMMAND IS ESPECIALLY          *   FILE 416
//*                 USEFUL FOR ENTERING RACF COMMANDS FROM          *   FILE 416
//*                 ISPF DIALOGS.  EX. DLXAUTHC LISTDSD             *   FILE 416
//*                 DA('DSN1.EXAMPLE') ALL                          *   FILE 416
//*                                                                 *   FILE 416
//*    EXIMPORT     GENERATE THE JCL NECESSARY FOR EXPORTING        *   FILE 416
//*                 AND IMPORTING THE DATA SETS ON A SPECIFIED      *   FILE 416
//*                 VOLUME.  CREATES ONE DATA SET WITH THE JCL      *   FILE 416
//*                 FOR EXPORTING THE DATA SETS ON A SPECIFIED      *   FILE 416
//*                 VOLUME AND ANOTHER FOR IMPORTING THE SAME       *   FILE 416
//*                 DATA SETS.  FOR VSAM FILES, THE JCL WILL        *   FILE 416
//*                 BE SET UP TO EXECUTE IDCAMS, EXPORTING TO       *   FILE 416
//*                 TAPE AND THEN IMPORTING BACK ONTO THE SAME      *   FILE 416
//*                 VOLUME FROM THE TAPE.  FOR NON-VSAM PS          *   FILE 416
//*                 FILES, THE PROGRAM IEBGENER IS EXECUTED TO      *   FILE 416
//*                 COPY THE DATA SET TO TAPE AND THEN BACK TO      *   FILE 416
//*                 THE SAME VOLUME.  FOR PO FILES, IEBCOPY IS      *   FILE 416
//*                 USED.  ALSO A CLIST IS GENERATED TO             *   FILE 416
//*                 SCRATCH THE TAPE FILES AFTER THE DATA SETS      *   FILE 416
//*                 HAVE BEEN IMPORTED.                             *   FILE 416
//*                                                                 *   FILE 416
//*    IGGPRE00     DF/DS ALLOCATE PRE PROCESSING EXIT              *   FILE 416
//*                 TESTER.                                         *   FILE 416
//*                                                                 *   FILE 416
//*    INMRZ01      RECEIVE INITIALIZATION EXIT ALLOWS              *   FILE 416
//*                 AUTHORIZATION CHECKING FOR USER IDS             *   FILE 416
//*                 EXECUTING RECEIVE IN BACKGROUND.                *   FILE 416
//*                                                                 *   FILE 416
//*    INMRZ11      RECEIVE PRE-PROCESSING EXIT ALLOWS RECEIVE      *   FILE 416
//*                 TO RUN IN BACKGROUND WITH THE EXIT              *   FILE 416
//*                 REPLACING THE USER INTERACTION IN               *   FILE 416
//*                 DETERMINING THE RECEIVING DATA SET NAME.        *   FILE 416
//*                                                                 *   FILE 416
//*    RACFALT   -  THIS PROGRAM WILL GENERATE A CLIST TO           *   FILE 416
//*                 CHANGE THE VOLUME SERIAL NUMBERS IN THE         *   FILE 416
//*                 RACF PROFILES OF ALL NONVSAM DATASETS ON A      *   FILE 416
//*                 SPECIFIED VOLUME.                               *   FILE 416
//*                                                                 *   FILE 416
//*    RACFCLST  -  THIS PROGRAM WILL GENERATE A CLIST TO           *   FILE 416
//*                 REDEFINE (VIA RACF COMMANDS DELDSD, ADDSD,      *   FILE 416
//*                 AND PERMIT) FOR ALL DATASETS ON A               *   FILE 416
//*                 SPECIFIED VOLUME.  DUE TO USE OF RACF           *   FILE 416
//*                 INTERNAL MACROS THIS PROGRAM MUST BE RUN        *   FILE 416
//*                 AUTHORIZED.  IF SYSIN IS PRESENT YOU CAN        *   FILE 416
//*                 INCLUDE COMMANDS TO SELECT BY DATASET           *   FILE 416
//*                 GROUP ON A VOLUME AND/OR DATASET NAME WITH      *   FILE 416
//*                 OR WITHOUT VOLUME SPECIFICATION.  WARNING:      *   FILE 416
//*                 IF SYSIN IS PRESENT AND DUMMIED OUT OR          *   FILE 416
//*                 EMPTY THEN A NULL CLIST WILL BE CREATED.        *   FILE 416
//*                                                                 *   FILE 416
```
