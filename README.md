# utl_create_your_own_dashboard_using_classic_base_sas
Create your own dashboard using just the classic editor and base SAS.  Keywords: sas sql join merge big data analytics macros oracle teradata mysql sas communities stackoverflow statistics artificial inteligence AI Python R Java Javascript WPS Matlab SPSS Scala Perl C C# Excel MS Access JSON graphics maps NLP natural language processing machine learning igraph DOSUBL DOW loop stackoverfl SAS community.
    Create your own dashboard using just the classic editor and base SAS

    Problem: Select the report you want to run from a dashboard.

    To see output dashboards

    https://tinyurl.com/y7f29k8q
    https://tinyurl.com/ydc2dbpb
    https://tinyurl.com/ya7o34of
    https://tinyurl.com/y9nmor86

    I doubt this will work in any 'enhanced' SAS editor ie EE, EG, UE, Studio ...
    This does not work in WPS.
    Probably need the sasfont(lowercase sasfont).

    see github project
    https://tinyurl.com/yc6n6rtg
    https://github.com/rogerjdeangelis/utl_create_your_own_dashboard_using_classic_base_sas


    * This is a WIN 95 ERA TIP (updated);

    INPUT  ( you need to design your dashboard using the powerfull classic DMS editor)
    ===================================================================================

      Macros are at the end of this message

      Type keys on the classic editor command line,
      then set function key 3 (PF3) to 'end;'

      Example of one of the four buttons

      values('                                                            ')
      values('ggggggggggggggggg     gggggggggggggggggg   gggggggggggggggg ')
      values('g            °  gr    g  „ƒƒƒ†         gr  g              gr')
      values('g CO       °  ° gr    g  Šƒ…ƒŒ     Rx  gr  g      •˜—     gr')
      values('g   ² •””””   ° gr    g  „ƒˆƒ†      ©  gr  g    •˜˜˜““—   gr')
      values('g     “    °° ° gr    g  ‡ƒ‹ƒ‰   ®     gr  g   ›˜œ™˜–œšŸ  gr')
      values('g  „ƒƒ“†    °   gr    g  ‡ppp‰  ®  ©   gr  g    “ ˜˜š “   gr')
      values('g  ‡bbb‰        gr    g  ‡ppp‰  ©  ©   gr  g    ˜–šœ˜–š   gr')
      values('g  ‡bbb‰  H O   gr    g  ‡ppp‰   ©     gr  g    ˜™š ˜™š   gr')
      values('g  ‡bbb‰   ²    gr    g  ŠƒˆƒŒ         gr  g    ›œŸ ›œŸ   gr')
      values('g  ŠƒƒƒŒ        gr    g    ‚           gr  g              gr')
      values('g     LABS      gr    g    CONMEDS     gr  g DEMOGRAPHICS gr')
      values('gggggggggggggggggr    ggggggggggggggggggr  ggggggggggggggggr')
      values(' rrrrrrrrrrrrrrrrr     rrrrrrrrrrrrrrrrrr   rrrrrrrrrrrrrrrr')
      values('                                                            ')
      values('    1                     2                   3             ')
      values('                                                            ')
      values('ggggggggggggggggggggggggggg    gggggggggggggggggggggggggggg ')
      values('g •”””””””—  •””””””””””— gr   g  „ƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒ†  gr')
      values('g “bbbbbbb“  “pppppppppp“ gr   g  ‚ppppp•”””””””—pppppp‚  gr')
      values('g “bSIGNSb“  “pSYMPTOMSp“ gr   g  ‚ppppp“ BAND  “pppppp‚  gr')
      values('g “bbbbbbb“  “pppppppppp“ gr   g  ‚ppppp“  AID  “pppppp‚  gr')
      values('g ›”””–”””Ÿ  ›””””–”””””Ÿ gr   g  ‚ppppp›”””””””Ÿpppppp‚  gr')
      values('g     “           “       gr   g  ŠƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒŒ  gr')
      values('g       SYMPTOMS          gr   g     ADVERSE  EVENTS      gr')
      values('gggggggggggggggggggggggggggr   ggggggggggggggggggggggggggggr')
      values(' rrrrrrrrrrrrrrrrrrrrrrrrrrr    rrrrrrrrrrrrrrrrrrrrrrrrrrrr')
      values('                                                            ')
      values('    4                                  5                    ')
      values('                                                            ')
      values('#32 @21 CHOICE 1 attr=rev_video @23 "Enter 1-5;"            ')
      values('                                                            ')

    PROCESS
    =======

       For the first dashboard Buttons 1;

       %utlbutn_display(butn=utlbutn1);

       Enter the number you want into the blinking black box then hit PF3

       Other dashboards

       %utlbutn_display(butn=utlbutn2);
       %utlbutn_display(butn=utlbutn3);
       %utlbutn_display(butn=utlbutn4);

    WANT DEMOGRAPHICS REPORT
    ========================

      If demographics button was selected you get this report

        You pressed 3 then PF3 in th eblinking box

                  S
                  E
        NAME      X        AGE     HEIGHT     WEIGHT
        Alfred    M         14         69      112.5
        Alice     F         13       56.5         84
        Barbara   F         13       65.3         98
        Carol     F         14       62.8      102.5
        Henry     M         14       63.5      102.5
        James     M         12       57.3         83
        Jane      F         12       59.8       84.5
        Janet     F         15       62.5      112.5
        Jeffrey   M         13       62.5         84
        John      M         12         59       99.5
        Joyce     F         11       51.3       50.5
        Judy      F         14       64.3         90
        Louise    F         12       56.3         77
        Mary      F         15       66.5        112
        Philip    M         16         72        150
        Robert    M         12       64.8        128
        Ronald    M         15         67        133
        Thomas    M         11       57.5         85
        William   M         15       66.5        112


    FULL SOLUTION
    =============

    When I wrote this there was not such thing as a dashboard
    so I used the term buttons

    %macro utlbutnm
         (
           utitle=Create your own dashboard,

           /*-------------------------------------*\
           |                                       |
           | ONLY WORKS WITH THE OLD TEXT EDITOR?  |
           |                                       |
           |  ONLY BASE SAS IS REQUIRED FOR THIS   |
           |  APPLICATION                          |
           |                                       |
           |  INPUTS                               |
           |  ======                               |
           |                                       |
           |  USER EDITED TEMPLATES ie             |
           |                                       |
           |    gggggggggggggggggg                 |
           |    g                gr                |
           |    g8‡              gr                |
           |    g ‡    x x   x   gr                |
           |    g6‡              gr                |
           |    g ‡     x  x     gr                |
           |    g4‡    x         gr                |
           |    g ‡  x           gr                |
           |    g2‡              gr                |
           |    g Š‹‹‹‹‹‹‹‹‹‹‹‹‹ gr                |
           |    g  1 2 3 4 5 6 7 gr                |
           |    ggggggggggggggggggr                |
           |     rrrrrrrrrrrrrrrrrr                |
           |                                       |
           |    g = heavy black line               |
           |    r = depth shading                  |
           |                                       |
           |   This app looks aweful on low res    |
           |   monitors. Must have sasfont.        |
           |                                       |
           |                                       |
           \*-------------------------------------*/

            uot1=d:\btn

           )
           / DES = "Create your own dashboard";


    libname uot "&uot1";

    proc datasets library=uot;
      delete utlbutn:;
    quit;

    proc sql;

      create
               table uot.utlbutn1
                       (
                        type =   data
                        label = 'Cards stmt not valid macro',

                        crd   char(63)  label="Edited Templates"

                       )
      ;

      insert
               into  uot.utlbutn1


      values('                                                               ')
      values(' ggggggggggggggggg    gggggggggggggggggg    gggggggggggggggggg ')
      values(' g               gr   gSAT SUN MON TUE gr   g                gr')
      values(' g         ooo   gr   gyyyybbbbccccoooogr   g8‡              gr')
      values(' g      pppooo   gr   gyyyybbbbccccoooogr   g ‡    x x   x   gr')
      values(' g      pppooo   gr   gyyyybbbbccccoooogr   g6‡              gr')
      values(' g   bbbpppooo   gr   gccccooooyyyybbbbgr   g ‡     x  x     gr')
      values(' g   bbbpppooo   gr   gccccooooyyyybbbbgr   g4‡    x         gr')
      values(' g   bbbpppooo   gr   gccccooooyyyybbbbgr   g ‡  x           gr')
      values(' gyyybbbpppooocccgr   gooooccccooooyyyygr   g2‡              gr')
      values(' gyyybbbpppooocccgr   gooooccccooooyyyygr   g Š‹‹‹‹‹‹‹‹‹‹‹‹‹ gr')
      values(' gyyybbbpppooocccgr   gooooccccooooyyyygr   g  1 2 3 4 5 6 7 gr')
      values(' gggggggggggggggggr   ggggggggggggggggggr   ggggggggggggggggggr')
      values('  rrrrrrrrrrrrrrrrr    rrrrrrrrrrrrrrrrrr    rrrrrrrrrrrrrrrrrr')
      values('                                                               ')
      values('   1                     2                      3              ')
      values('                                                               ')
      values('ggggggggggggggggggggggggggg     gggggggggggggggggggggggggggggg ')
      values('g„ƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒ†gr    g„ƒƒƒƒƒƒƒƒƒƒ…ƒƒƒ…ƒƒƒ…ƒƒƒ…ƒƒƒ†gr')
      values('g‚REPORT   A   B   C   D ‚gr    g‚TABULALATE‚  A‚  B‚ C ‚ D ‚gr')
      values('g‡ƒƒƒƒƒƒƒ…ƒƒƒ…ƒƒƒ…ƒƒƒ…ƒƒƒ‰gr    g‡ƒƒƒƒƒƒƒƒƒƒˆƒƒƒˆƒƒƒˆƒƒƒˆƒƒƒ‰gr')
      values('g‚ AGE   ‚   ‚   ‚   ‚   ‚gr    g‚ AGE      ‚   ‚   ‚   ‚   ‚gr')
      values('g‡ƒƒƒƒƒƒƒˆƒƒƒˆƒƒƒˆƒƒƒˆƒƒƒ‰gr    g‡ƒƒƒƒƒƒƒƒƒƒˆƒƒƒˆƒƒƒˆƒƒƒˆƒƒƒ‰gr')
      values('g‚ SEX   ‚   ‚   ‚   ‚   ‚gr    g‚ SEX      ‚   ‚   ‚   ‚   ‚gr')
      values('gŠƒƒƒƒƒƒƒ‹ƒƒƒ‹ƒƒƒ‹ƒƒƒ‹ƒƒƒŒgr    gŠƒƒƒƒƒƒƒƒƒƒ‹ƒƒƒ‹ƒƒƒ‹ƒƒƒ‹ƒƒƒŒgr')
      values('gggggggggggggggggggggggggggr    ggggggggggggggggggggggggggggggr')
      values(' rrrrrrrrrrrrrrrrrrrrrrrrrrr     rrrrrrrrrrrrrrrrrrrrrrrrrrrrrr')
      values('                                                               ')
      values('    4                                  5                       ')
      values('                                                               ')
      values('#32 @21 CHOICE 1 attr=rev_video @23 "Enter 1-5;"              ')
      values('                                                              ')
    ;

      create
               table uot.utlbutn2
                       (
                        type =   data
                        label = 'Cards stmt not valid macro',

                        crd   char(63)  label="Edited Templates"

                       )
      ;

      insert
               into  uot.utlbutn2


      values('                                                            ')
      values('ggggggggggggggggg     gggggggggggggggggg   gggggggggggggggg ')
      values('g            °  gr    g  „ƒƒƒ†         gr  g              gr')
      values('g CO       °  ° gr    g  Šƒ…ƒŒ     Rx  gr  g      •˜—     gr')
      values('g   ² •””””   ° gr    g  „ƒˆƒ†      ©  gr  g    •˜˜˜““—   gr')
      values('g     “    °° ° gr    g  ‡ƒ‹ƒ‰   ®     gr  g   ›˜œ™˜–œšŸ  gr')
      values('g  „ƒƒ“†    °   gr    g  ‡ppp‰  ®  ©   gr  g    “ ˜˜š “   gr')
      values('g  ‡bbb‰        gr    g  ‡ppp‰  ©  ©   gr  g    ˜–šœ˜–š   gr')
      values('g  ‡bbb‰  H O   gr    g  ‡ppp‰   ©     gr  g    ˜™š ˜™š   gr')
      values('g  ‡bbb‰   ²    gr    g  ŠƒˆƒŒ         gr  g    ›œŸ ›œŸ   gr')
      values('g  ŠƒƒƒŒ        gr    g    ‚           gr  g              gr')
      values('g     LABS      gr    g    CONMEDS     gr  g DEMOGRAPHICS gr')
      values('gggggggggggggggggr    ggggggggggggggggggr  ggggggggggggggggr')
      values(' rrrrrrrrrrrrrrrrr     rrrrrrrrrrrrrrrrrr   rrrrrrrrrrrrrrrr')
      values('                                                            ')
      values('    1                     2                   3             ')
      values('                                                            ')
      values('ggggggggggggggggggggggggggg    gggggggggggggggggggggggggggg ')
      values('g •”””””””—  •””””””””””— gr   g  „ƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒ†  gr')
      values('g “bbbbbbb“  “pppppppppp“ gr   g  ‚ppppp•”””””””—pppppp‚  gr')
      values('g “bSIGNSb“  “pSYMPTOMSp“ gr   g  ‚ppppp“ BAND  “pppppp‚  gr')
      values('g “bbbbbbb“  “pppppppppp“ gr   g  ‚ppppp“  AID  “pppppp‚  gr')
      values('g ›”””–”””Ÿ  ›””””–”””””Ÿ gr   g  ‚ppppp›”””””””Ÿpppppp‚  gr')
      values('g     “           “       gr   g  ŠƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒŒ  gr')
      values('g       SYMPTOMS          gr   g     ADVERSE  EVENTS      gr')
      values('gggggggggggggggggggggggggggr   ggggggggggggggggggggggggggggr')
      values(' rrrrrrrrrrrrrrrrrrrrrrrrrrr    rrrrrrrrrrrrrrrrrrrrrrrrrrrr')
      values('                                                            ')
      values('    4                                  5                    ')
      values('                                                            ')
      values('#32 @21 CHOICE 1 attr=rev_video @23 "Enter 1-5;"            ')
      values('                                                            ')
    ;

      create
               table uot.utlbutn3
                       (
                        type =   data
                        label = 'Cards stmt not valid macro',

                        crd   char(63)  label="Edited Templates"

                       )
      ;

      insert
               into  uot.utlbutn3

      values('                                                            ')
      values('ggggggggggggggggggggggggggg    gggggggggggggggggggggggggggg ')
      values('g •”””””””—  •””””””””””— gr   g  „ƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒ†  gr')
      values('g “bbbbbbb“  “pppppppppp“ gr   g  ‚ppppp•”””””””—pppppp‚  gr')
      values('g “bORACLE“=>“pANDYppppp“ gr   g  ‚ppppp“       “pppppp‚  gr')
      values('g “bAEAEbb“  “pLAWTONppp“ gr   g  ‚ppppp“       “pppppp‚  gr')
      values('g “bSASbbb“  “pADVERSEpp“ gr   g  ‚ppppp“ BAND  “pppppp‚  gr')
      values('g “bVIEWbb“=>“pEVENTpppp“ gr   g  ‚ppppp“  AID  “pppppp‚  gr')
      values('g “bbbbbbb“  “pTABLEpppp“ gr   g  ‚ppppp“       “pppppp‚  gr')
      values('g “bbbbbbb“  “pppppppppp“ gr   g  ‚ppppp“       “pppppp‚  gr')
      values('g ›”””””””Ÿ  ›””””””””””Ÿ gr   g  ‚ppppp›”””””””Ÿpppppp‚  gr')
      values('g                         gr   g  ŠƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒƒŒ  gr')
      values('g  STANDARDIZE ANALYSIS   gr   g   ADVERSE EVENT REPORTS  gr')
      values('g  ADVERSE EVENT TABLES   gr   g   PRINT MACRO READY      gr')
      values('g  USING LAWTON STANDARDS gr   g   USING LAWTON STANDARD  gr')
      values('gggggggggggggggggggggggggggr   ggggggggggggggggggggggggggggr')
      values(' rrrrrrrrrrrrrrrrrrrrrrrrrrr    rrrrrrrrrrrrrrrrrrrrrrrrrrrr')
      values('                                                            ')
      values('          1                                 2               ')
      values('                                                            ')
      values('                                                            ')
      values('#32 @21 CHOICE 1 attr=rev_video @23 "Enter 1 or 2;"         ')
      values('                                                            ')
    ;

      create
               table uot.utlbutn4
                       (
                        type =   data
                        label = 'Cards stmt not valid macro',

                        crd   char(63)  label="Edited Templates"

                       )
      ;

      insert
               into  uot.utlbutn4

      values('                                                        ')
      values('                                                        ')
      values('                    gggggggggggggggggggg                ')
      values('                    g                  gr               ')
      values('                    g       •˜—        gr               ')
      values('                    g     •˜˜˜““—      gr               ')
      values('                    g    ›˜œ™˜–œšŸ     gr               ')
      values('                    g     “ ˜˜š “      gr               ')
      values('                    g     ˜–šœ˜–š      gr               ')
      values('                    g     ˜™š ˜™š      gr               ')
      values('                    g     ›œŸ ›œŸ      gr               ')
      values('                    g                  gr               ')
      values('                    g                  gr               ')
      values('                    ggggggggggggggggggggr               ')
      values('                     rrrrrrrrrrrrrrrrrrrr               ')
      values('                                                        ')
      VALUES('                                                        ')
      VALUES('#18 @21 CHOICE 1 attr=rev_video @23 "ENTER Y/N;"        ')
      VALUES('                                                        ')
      values('                                                        ')
    ;

    quit;

    %mend utlbutnm;


    %utlbutnm;          1


    %macro utlbutnx(uotbutn=utlbutn1,uot=d:/btn);

    %let a=%str(attr=rev_video);   /*-------------------------------------*/
    %let b=%str(color=brown);      /* Change these color defs             */
    %let g=%str(color=black);      /* for less bright hues                */
    %let y=%str(color=yellow);     /*-------------------------------------*/
    %let c=%str(color=cyan);
    %let b=%str(color=blue);
    %let p=%str(color=pink);
    %let r=%str(color=red);
    %let o=%str(color=orange);
    %let w=%str(color=white);
    %let f=%str(color=grey);
    %let m=%str(color=magenta);
    %let j=%str(color=green);

    libname uot clear;
    filename utlbutn catalog ;

    LIBNAME UOT "&uot.";

    proc catalog cat=sasuser.utlbutn;
      delete &uotbutn..catams;
    run;quit;

    filename utlbutn catalog "sasuser.utlbutn.&uotbutn..catams";

    data _null_;


       retain ques 0;

       file utlbutn;

       set uot.&uotbutn;


       %do ui = 1 %to 63;

          c&ui = substr(crd,&ui,1);

       %end;

       array chars{63} $ 1 c1-c63;

      if _n_ eq 1 then

           put '%window ' "&uotbutn "  'color=white  columns=65 rows=44';

       do i=1 to 63;

          select ( chars{i} ) ;

              when(  '#' ) do; put crd; i=63; end;

              when ( '?' )  do;

                   ques+1;
                   box='box'!!compress(put(ques,1.));
                   put '#' _n_ '@' i  box +2 ques "  12 &a &g";

              end;

              when ( 'g' )
                   put '#' _n_ '@' i "' ' &a &g";
              when ( 'r' )
                   put '#' _n_ '@' i "' ' &a &f";
              when ( 'j')
                   put '#' _n_ '@' i "' ' &a &j";
              when ( 'y' )
                   put '#' _n_ '@' i "' ' &a &y";
              when ( 'b')
                   put '#' _n_ '@' i "' ' &a &b";
              when ( 'c' )
                   put '#' _n_ '@' i "' ' &a &c";
              when ( 'p')
                   put '#' _n_ '@' i "' ' &a &p";
              when ( 'o')
                   put '#' _n_ '@' i "' ' &a &o";
              otherwise
              if chars{i} ne ' ' then
                   put '#' _n_ '@' i '"' chars{i} $1. '"';
                        else;
          end;

      end;

    run;

    %do ui = 1 %to 9;

      %let box&ui =Click Me;

    %end;

    run;quit;

    libname uot clear;
    filename utlbutn catalog;

    %mend utlbutnx;

    %utlbutnx(uotbutn=utlbutn1);
    %utlbutnx(uotbutn=utlbutn2);
    %utlbutnx(uotbutn=utlbutn3);
    %utlbutnx(uotbutn=utlbutn4);

    %macro utlbutn_display(butn=utlbutn2,uin=d:/btn);

    %do ui = 1 %to 9;

      %let box&ui =Click Me;

    %end;

      /*
      %let butn=utlbutn4;
      %let uin=d:/btn;
      */
      libname ui clear;
      filename fileref1 catalog;

      libname uin "&uin";

      filename fileref1 catalog "sasuser.utlbutn.&butn..catams";
      run;quit;

      %include fileref1;
      run;quit;

      %symdel choice;

      %display  &butn;
      ;run;quit;

      %if "&choice" ne "" %then %do;
        proc report data=sashelp.class nowd;
        run;quit;
      %end;

      libname uin clear;
      filename fileref1 catalog;
      run;quit;

    %mend utlbutn_display;

