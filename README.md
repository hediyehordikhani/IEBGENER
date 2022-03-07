# IEBGENER
JCL CODE
//JOBNAME JOB ,'ZEINAB ORDIKHANI',NOTIFY=DBKIZO1                        
//STEP1 EXEC PGM=IEBGENER                                               
//SYSIN DD DUMMY                                                        
//SYSPRINT DD SYSOUT=X                                                  
//SYSUT1 DD DSN=DBKIZO1.IEFBR14.TEST,DISP=SHR                           
//SYSUT2 DD DSN=DBKIZO1.IEFBR14.CRE,                                    
//          DISP=(NEW,CATLG,DELETE),                                    
//          SPACE=(TRK,(2,2),RLSE),                                     
//          DCB=(RECFM=FB,LRECL=80,BLKSIZE=800)  
