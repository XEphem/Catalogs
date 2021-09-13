# v3.7                  Database Directory Structure               (CSI, 2005)
# ============================================================================
#      By Elwood Charles Downey. (c)2000 Clear Sky Institute.
#      If you have  inquires regarding the use and/or modification of the
#      dataset  described  in this file  and contained  in this directory,
#      in part or as a whole, please contact Elwood Downey, President/CEO, 
#      Clear Sky Institute, Inc. ecdowney@clearskyinstitute.com
# ============================================================================
# Version of this Document: July 15th 2005, by G.A.
# ____________________________________________________________________________
# 
#                             Table of Contents
# 
#     1. Designation Rules.
#     2. Supplied Databases.
#     3. Warnings and Disclaimer.
#     4. Directory Structure.
#     5. Database Description.
#     6. IAU Recommendations for Nomenclature.
# 
# Note:
# This file contains a general and  brief description to the updates and major
# changes occured into the /catalogs subdirectory.
# 
# ____________________________________________________________________________
#
# 1. Designation Rules.
# 
# This is a  collection of files in XEphem database format.  Included here are
# asteroids, comets, stars, deep-sky objects, earth satellites and spacecraft.
# Work on the databases is  a major project in itself. There  are  bound to be
# errors. Authoritative contributions are welcome.
# The naming conventions chosen for this directory are straightforward:
# 
#     A. Databases  known better by its author are named after his/her
#        lastname, beggining with a capital letter.
#     B. Databases with a high degree of autonomy and independence and
#        general purpose usability in respect of the data they include,
#        are  normally  written  with their respective acronyms in all 
#        capital letters.
#     C. In  some  cases  you'll  find  two  (2)  versions of the same
#        database.  This  is  normally  due  to  the  use  of  special
#        designations  of  the  objects included.  The positional data
#        itself should be exactly equal for both of them.
#        When this happens (such as with YBS.edb and YBS-O.edb), it is 
#        allowed to use this suffix:
#          -O Indicating "Original" designations to whatever the 
# 	    catalog had used originally with its objects.
# 	    This implies following the IAU rules in respect of
# 	    designations whenever possible. This also  implies 
# 	    the existance of another database with  common  or
# 	    alternate designations, meaning "Common" Names for 
# 	    objects already included.
#     D. Special databases, according to different criteria, are named
#        with non-capital letters (i.e bs.edb).
#     
# ===========================================================================
# 2. Supplied Databases.
# 
#   If you have purchased the 3.7 version of XEphem, you'll probably have
# available many databases that may be not readily present for the rest of
# the users who have chosen instead only to download the 'free' binaries.
#   Part of this directory will be familiar to prior users.
#   A little part of it should be new for everyone!
#   
#   For some time now we have been revising and  updating the data as much
# as it has been possible, keeping in mind to offer the best tools for
# all XEphem's users: professional and amateurs alike.  This involved
# the testing and verification of many of  the enclosed datasets, in the
# extent that our time permitted us, resulting  in a  hopefully better 
# collection of references and information tools for our users.
# 
#   In the light of the datasets, which may include several "new" .edb 
# format features (such as multiple designations, multiple spectral types,
# two-char descriptors etc.) the best policy to treat all previous version
# installations is to fully erase the old 'catalogs' directory.
# 
#   Many of the old files (i.e. ldn.edb) were completely revised and re-
# generated from scratch, adding some new features in the way. For
# example, the old hickson.edb now is named "Hickson.edb" and, in
# comparison to the previous version that showed the positional data for
# its 100 components, it presently includes morphological data, full
# componenent positional categories, multiple designations etc.
# 
#   Your custom .edb should keep working as usual.
# 
# ===========================================================================
# 3. Some Warnings.
# 
#    DISCLAIMER: Along the update and inclusion of the data, we have always
#    tried to maintain a strict policy  in accepting or including new data-
#    bases. We  feel  an  obligation for  all XEphem users for  keeping and
#    offering the best  scientific-grade  data  publicly available  and, in
#    this respect, the  naming  convention  for  all objects, with the sole
#    exception  of  our Deep  Sky Common Name database, should follow known
#    guidelines  in  the  international  community  in  order  to  obtain a 
#    systematic homogeneity:   the  rules   of  the  Standarized  List  for
#    Online Databases given by the Astronomical Catalog Desginations of the
#    IEE, the Second Reference Dictionary  of the Nomenclature of Celestial
#    Objects by Lortet et.al.  Publication  Speciale du C.D.S., No.24, Vol.
#    I, II,  1994.,  and  the results of the Working  Group for Information 
#    Retrieval of Commision 5 of the International Astronomical Union (IAU),
#    gave us the framework from which we could re-evaluate our own level of
#    compliance. We feel that we have, insofar, made what  was  necesary to
#    address some  of  the most significant problems in this area, although 
#    there's still much work to do yet.
# 
#    There */ may /* be  many  innacuracies  remaining  in  some  databases
#    but, all in all, we are certain that our present overall structure and
#    organization, as well as the chosen nomenclature, both in their origi-
#    nal  (-O)  and   modified   forms  represent excellent tools for  com-
#    plementing the wealth of functions available within XEphem for all the 
#    serious amateurs and researchers around the world.
# 
#    We are not responsible for erroneous designations coming from the data
#    authors! Whenever possible we did try to prevent and correct such pro-
#    blems in advance but, as said, this task is by no means simple or sho-
#    rt. There may still be many inacuracies or deficiencies in the  object
#    positional data and/or its designation and/or its classification. 
#    Nonetheless,as far as we are aware of, the relationship between actual
#    and  valid data against the erroneous information should tend to favor 
#    the former.
# 
#    Clear Skies!!!
# 
#    E.D. & G.A.
# ===========================================================================
# 
# 4. Structure.
#    		                 XEphem 3.7
# 			     Commercial Version
# 		       Database Directory Description
# 		     ----------------------------------
#
# The /catalogs directory should contain the following databases listed in no 
# particular  order.  The classification shown is completely arbitrary and it
# is  *not*  mandatory  to any user, or  to  be  taken  as  a  reference. Its
# implementation  was  born  out  of  a  practical  need   to  categorize the
# many sources available with standard commercial XEphem, and present them in 
# a more logical way.
#   Please  bear in mind that previous versions  (3.52 and below) of the same 
# databases are *not*  to be used or combined with the new version. There may
# be some degree of  incompatability  that  the users should avoid by erasing
# the old installation in the /shared/ directory before entering the 3.7.
#   Also, many of the new versions shown herein are *not* compatible  and can 
# not be read by older versions of XEphem than 3.6.
#
# Current number of officially distributed catalogs to date (Aug/1/2005) (not 
# including field stars): 42.
# 
# 1. General Purpose:
#    a) SKY2000 Master Catalog v.4, 2002. ---------->  SKY2000.edb
#    b) SKY2000 Bright Stars Subset, 2002. --------->  SKY2k65.edb
#    c) Revised New General Catalog, 2005. ------------->  NGC.edb
#    d) Revised Index Catalog, 2005. -------------------->  IC.edb
#    e) XZ Catalog of Zodiacal Stars, 2003. ---------->  XZ80Q.edb
#    f) Saguaro Astronomy Club Database 7.2, 2002. ->  Saguaro.edb
#    g) Messier Objects Catalog, 2005. ------------->  Messier.edb
# 
# 2. Field Stars:
#    a) USNO SA2.0 image Catalog.------------------------>  /usno
#    b) GSC-ACT Catalog. --------------------------------->  /gsc
#    c) Hipparcos and Tycho-2 Catalogues. ---------->  hiptyc2.xe2
#    d) Positions in Proper Motions Catalog. ----------->  ppm.xe2
# 
# 3. Galaxies and Clusters of Galaxies:
#    a) HYPERLEDA Catalogue, 2003 (p.1, bright).-->  HYPERLEDA.edb
#    b) HYPERLEDA Catalogue, 2003 (p.2, dim).->  HYPERLEDA_dim.edb
#    c) Hickson Objects Catalog, 1994. ------------->  Hickson.edb
#    d) Galaxies and Clusters of Galaxies Catalog. ---->  cgcg.edb
#    e) Uppsala General Catalog. ----------------------->  UGC.edb
#    f) Abell Clusters of Galaxies Catalogue, 1989. -->  Abell.edb
# 
# 4. Bright Nebulae, Dark Nebulae and similar objects:
#    a) Lynds' Catalogue of Bright Nebulae, 1965.------->  lbn.edb
#    b) Lynds' Catalogue of Dark Nebulae, 1962. -------->  ldn.edb
#    c) Barnard's Catalogue of Dark Objects, 1927. ->  Barnard.edb
#    d) A Catalogue of Southern Dark Clouds, 1986. ---->  DCld.edb
#    e) Catalog of Galactic Supernova Remnants, 2001.-->  cgsr.edb
#    f) Sharpless Catalogue of HII regions, 1959. ------>  sh2.edb
# 
# 5. Observation oriented Catalogs:
#    a) Sternberg Supernova Catalogue, 2004. ----------->  SSC.edb
#    b) Quasars and AGN Catalog 11th Ed., 2003 -------->  qagn.edb
#    c) General Catalog of Variable Stars. ------------>  gcvs.edb
#    d) AAVSO Stars Catalog -------------------------->  aavso.edb
#    e) Optically Visible Open Clusters Catalog, 2002 >  ovocc.edb
# 
# 6. Binary Systems Catalogs:
#    a) Washington Visual Double Star Catalog, 2005 --->  WDSC.edb
#    b) Sixth Catalog of Orbits of Visual Binary Stars-> COVBS.edb
#    c) WDS Binary Star Calibration List,2004.->  binary_calib.edb
#    d) CCDM-Components of Double and Multiple Stars. ->  CCDM.edb
# 
# 7. Calibration and Photometry Catalogs:
#    a) VLA Radio Calibrator Sources. --------------->  vla*cm.edb
#    b) LONEOS Photometry Catalog, 2003.------------->  loneos.edb
#    c) The Updated Zwicky Catalog 1999. ------------>  Zwicky.edb
#    d) Catalog of Constant Brightness Stars,1997. >  constant.edb
#    e) WDS Single Star Calibration Cat.,2004.-->  sstar_calib.edb
#    f) USNO IR Stellar Sources Cat.CPIRSS. 1984. --->  CPIRSS.edb
#
# 8. Comets and Asteroids:
#    a) Minor Planet Center, asteroids to Mag 13 -----> AstMPC.edb
#    b) Minor Planet Center, dimmer than 13  -----> AstMPC_dim.edb
#    c) Lowell Observatory, asteroids to Mag 13 ---> AstLowell.edb
#    d) Lowell Observatory, dimmer than 13  ---> AstLowell_dim.edb
#    e) Observable comets, courtesy CFA, 2005 --------> comets.edb
# 
# 9. Other Catalogs:
#    a) Pulsars List ------------------------------->  pulsars.edb
#    b) Spacecraft catalog ---------------------->  spacecraft.edb
#    e) Deep Sky Objects Common Names, 2003. ----->  DeepSky-C.edb
#    c) Bright Star catalog ----------------------------->  bs.edb
#    d) Nautical Almanac Nav Stars.--------------------->  nav.edb
#    e) Henry Draper Catalog and Extension, 1924 -------->  hd.edb
#    f) Henry Draper Extension Charts, 1995 ------------>  hde.edb
#    g) Pleiades field Membership, 1995 ----------->  pleiades.edb
#    h) Herbig-Haro Objects ------------------------------> hh.edb
#    i) Pulkovo catalogue ---------------------------> Pulkovo.edb
# ___________________________________________________________________________
# 
# *  We  are  planning  to  expand  this  list  with  many  new datasets that
# become  recently  available  to  the  public.  Hopefully,  any advance over
# this matter will be made known through our website at www.xephem.com.
# 
# ** If  you'd  like to  make a data contribution, please let us know. We are
# always open to recieve new datasets, provided it has been validated against 
# its  original  source, the  level of redundancy it represents  with  XEphem
# existing datasets is low, and some other criteria.
#    If, after reading this, you are still motivated, please  follow  the IAU 
# designation guidelines shown at the end of this document. 
# 
# ===========================================================================
# 
# 5. Brief Catalogues Description. 
# 
# Please read the comments at the beggining of the file you are interested in
# for further information. XEphem provides a new facility to perform this  at
# the Main Window-->Data-->Files-->Header button. These are called XCN or
# 'XEphem Catalog Notes'.
#
# When possible, we  provide the Coded Reference of the catalogs, used by The
# Second Reference  Dictionary  of  the  Nomenclature of Celestial Objects by
# Lortet et.al.  Publication Speciale du C.D.S., No.24, Vol. I, II, 1994., in
# the Table of Acronyms and the Table of Comprehensive Catalogues. 
# There may be a mention regarding original author and publication date.
# ___________________________________________________________________________
# 
# 6. IAU Recommendations for Nomenclature.
# ===========================================================================
# Ascii version of World Wide Web presentation of the 
# IAU Recommendations for Nomenclature 
# which is based upon LaTex version 1.7 26 January 1995 
# The latter does not include the Table of Contents but it
# has some of the text in bold and italics for emphasis.
# 
# Address comments to: 
# Prof. Helene R. Dickel 
# Chair of the Task Group on Designations of IAU Commision 5 
# Internet:  lanie@astro.uiuc.edu
# ---------------------------------------------------------------------------
# 
# Specifications concerning designations 
# for astronomical radiation sources outside the solar system 
# 
# Contents 
#  1. General Recommendations
#     All source listings should always contain positional information and/or 
#     a second designation next to a principal designation.
#  2. Case of existing designations
#  3. Creation of new designations 
#       Acronym 
#       Sequence 
#          Use of coordinates 
#       Specifier 
#       Punctuation and special characters 
#       Examples 
#          Examples of complete designations 
#          Examples of improper designations 
#  4. Advice on designations 
#  5. Further information 
# 
# Both latex and DVI versions of this document are accessible by anonymous
# ftp at node cdsarc.u-strasbg.fr 
# 
# Specifications concerning designations 
# for astronomical radiation sources outside the solar system 
# 
# Short title:  IAU Recommendations for Nomenclature 
# Keywords:     Designations IAU   
#  
#    	                    (version 23 January 1995) 
# ...........................................................................
# 
# A look at the current literature reveals that unclear, ambiguous or 
# confusing designations of astronomical sources of radiation are too often 
# encountered. 
# Therefore, all contributors to databases, and authors of papers, catalogues
# and surveys,  are  urged  to  adhere to the following set of specifications 
# (developed and endorsed by the International Astronomical Union); otherwise
# significant data may be irretrievably lost. 
# 
# 
# 1. General recommendations
# 
# All source  listings  should always contain positional information and/or a
# second designation next to a principal designation in order to avoid 
# ambiguities that can arise with a single designation.
# 
# 
# 2. Case of existing designations
# 
#    > When existing  designations are used in listings, they should never be 
#      altered (e.g., neither truncated nor rounded, nor shortened). 
#    > In  a  publication,  the  bibliographical reference of the designation 
#      should be given. 
# 
# 3. Creation of new designations
# 
# The  designation  of an astronomical source should consist of the following 
# parts : 
# 
#  		Acronym^Sequence^(Specifier) 
# 
#    Note that the ^ is used here to denote a blank. It  is used for emphasis
# in showing where spaces occur in a designation.  (Users are expected to use
# an actual blank  and not  this character.)  Parentheses  are  required if a 
# specifier  is  included.  Acronym  and sequence are essential, specifier is 
# optional; the  number  of blanks may be larger in machine-readable files to
# right justify numerical or tabular data. 
# 
#    The  following  examples illustrate the recommended form of astronomical 
# designations : 
# 
# 	NGC^205 
#  	PKS^1817-43 
#  	CO^J0326.0+3041.0 
#  	H2O^G123.4+57.6^(VLSR=-185)
#  	3CR^196 
# 
# 
# 3.1 Acronym
# 
# The acronym (earlier called origin) is a code (i.e.,  alphanumerical string  
# of characters) that specifies the catalog or collection of  sources. It may 
# be constructed  from catalog  names (e.g., NGC, BD),  the names of authors, 
# (RCW) instruments or observatories used (VLA, IRAS, 3C, 51W), etc. 
# 
#    The following rules apply to the construction of new acronyms: 
# 
#    > an acronym shall consist of at least three characters. 
# 
#    > an acronym  shall  consist  of  letters  and/or numerals only; special 
#      characters, including  superscripts , subscripts, and blanks should be 
#      avoided.
#    > an acronym shall be unique, i.e., the appropriate reference literature
#      (especially the Second Dictionary of Nomenclature -- see below) should
#      be checked  to  avoid  duplication with existing catalog designations,
#      constellation names, abbreviations of source types, etc. 
# 
#    > The title of a catalog shall include the acronym by which it is to be
#      known, [e.g., Fifth Fundamental Catalogue (FK5)].
# 
#    > Avoid excessively long acronyms. Conversely, users shall  never abbre-
#      viate an acronym. 
# 
# 
# 3.2 Sequence
# 
# The  sequence  (or numbering)  is  an  alphanumeric  string  of characters,
# normally only numerical,  that  uniquely  determines  the  source  within a
# catalog  or collection. It may be a sequence number within a catalog (e.g.,
# HD^224801), a combination of fields, or it may be based on coordinates. 
# 
# 
# 3.2.1 Use of coordinates
# 
# Coordinate-based  designations  are  just "names"  and  should  have enough
# significant figures to unambiguously identify the sources.  It  is expected
# that precise coordinates will be provided in the paper  (e.g., in a table),
# accompanied by any needed explanations and other relevant information.
# 
#    If  coordinates  in any form are used to encode a source of radiation, a 
# set of rules applies,  which  we  will illustrate with a source, namely the 
# QSO with coordinates: 
# 
#         (B1950.0)    RA = 00h 48m 48.97s   DEC = -42deg42' 52.1"       
#         (J2000.0)    RA = 00h 51m 09.38s   DEC = -42deg26' 33.8" 
# 
#    > A designation involving only coordinates, often improperly referred to 
#      in the literature  as an "IAU designation", is not sufficient to iden- 
#      tify a source unambiguously. An acronym should also be given.
#  
#    > Equatorial  coordinates  shall always be preceded by J if they are for 
#      the new standard equinox  of J2000.0 (i.e., IAU 1976 FK5-based, Julian
#      equinox  2000.0  system). They should be preceded by B if they are for 
#      the old  standard equinox  of B1950.0 (i.e., Bessel-Newcomb FK4-based,
#      Besselian  equinox  1950.0  system).   Galactic  coordinates  shall be 
#      preceded by a G.  The absence of code at the beginning of recognizable
#      equatorial coordinates will be interpreted,by default, as a missing B. 
# 
#      Ex: QSO^004848-4242.8 = QSO^B004848-4242.8 = QSO^J005109-4226.5
# 
#      A   galactic-based  designation  is  inappropriate  for  extragalactic
#      sources such as a QSO.  Examples  of  galactic-based  designations for 
#      sources  within  the  Milky  Way Galaxy may be found in section 3 (Ex.
#      H2O) and section 3.5.1 (Ex. PN).
#
#    > The "flag" letters J, B, and G  have  a special role : the flag letter
#      should immediately  precede the  coordinates  and  should be separated
#      from the acronym by a space (^). This space is particularly important,
#      as there are acronyms ending with J, B, and G. 
#  
#    > Coordinates shall contain leading zeroes (in RA and DEC) and  the plus
#      or minus sign : +BB.bb or -BB.bb, +DDMMSS.s or -DDMMSS.s 
# 
#    > Coordinates  shall  be  specified  as LLL.ll+BB.bb or LLL.ll-BB.bb for
#      galactic coordinates, and as  HHMMSS.ss+DDMMSS.s or HHMMSS.ss-DDMMSS.s
#      for equatorial coordinates (without spaces); fewer digits  may be used
#      as appropriate. 
# 
#      Ex: QSO^004848-4242.8 could have been designated by QSO^0048-427 or
#          QSO^0048-42 
# 
#    > Coordinates using an even number of digits (in either RA or DEC),fewer
#      than seven,  are  expressed  in the  sexagesimal system. The sequences
#      HHMM.mm  or  DD.dd  where  mm  and dd are decimal parts of a minute or
#      degree, respectively, should be avoided. If the number of digits is
#      odd and fewer than six, the right-most digit represents a decimal part
#      of hours, degrees or minutes (as, e.g., in the PKS-style HHMM+DDd or 
#      in IRAS source designation HHMMm+DDMM) and not tens of minutes or 
#      seconds (e.g. the formats HHMMS or +DDM should be avoided). If the
#      number of digits is more than six, the digits in excess of six are 
#      decimal parts of seconds of time for RA or of angle for DEC;  explicit
#      use of the decimal points is encouraged (e.g. HHMMSS.ss or DDMMSS.s). 
# 
#    > Coordinates shall be truncated (not rounded), thus defining a unique
#      (small) field on the sky in which the source is located.The truncation
#      should also operate when the right-most digit represents a decimal
#      part. The right-most digit of the field HHMMm should be computed as
#      m=int(SS/6). The same should be done when transforming from +DDMM to
#      DDd (as in the PKS-style) with d=int(MM/6). 
# 
#      Ex: QSO^004848-4242.8 could be named QSO^00488-4242 but not
#      QSO^00484-4242 (wrong truncation of RA) nor QSO^00488-4243 (rounded
#      DEC).
#
#    > Designations that include coordinates shall be treated as proper 
#      names; therefore, they shall not be changed even if the positions
#      change or become more accurately known. 
# 
#      Ex: BD^+25^9 stays, even though its declination has now changed to 
#      +26 degrees due to precession from its original position (at the 1855 
#      equinox). 
# 
# 
# 3.3 Specifier
# 
# The specifier is optional and allows one to indicate other source 
# parameters. However, they are not required syntax and are enclosed in
# parentheses. 
# 
# 3.4 Punctuation and special characters
# 
# If the  designation  requires the use of punctuation or special characters,
# the recommendations are the following : 
# 
# " " (blank character)should be used as separator rather than a ".", or "/". 
# 
# "_" (underscore) may be used in place of a blank, if necessary, such as
#     within an electronic catalog.
# 
# "-" should be reserved for the minus sign as much as possible. However, if
#     there is no ambiguity with the minus sign, then it may be used as a
#     separator although such useage is discouraged.
#  
# "." should be reserved for a decimal point.
#  
# "/" should be used for concatenation of the sources quoted. 
# 
#   	Ex: DR^21/23 refers to DR^21 and DR^23, not (DR^21, DR^22, DR^23) 
# 
# ":" should be reserved to indicate subdivision (subcomponent). 
# 
#    If at some stage subcomponents or multiplicity of sources is recognized, 
# the  best designation solution is to name the subcomponents with letters or 
# numerals, which then are added to the sequence with a colon; 
# e.g., NGC^1818:B^12. 
# 
# 
# 3.5 Examples
# 
# 3.5.1 Examples of complete designations
# 
# 	      Designation                        Position   
# 	Acronym^Sequence^(Specifier)      RA(J2000.0)    DEC(2000.0)
# 
# 	BD^-3^5750                       00 02 02.4      -02 45 59 
# 	PSR^J1302-6350			 13 02 47.72     -63 50 08.5
# 	AC^211^(=1E^2127+119; M^15)      21 30 15.54     +11 43 39.0 
# 	PN^G001.2-00.3                   17 49 36.9      -28 03 59 
# 	R^136:a3^(30^Dor)                05 38 42.4      -69 06 03 
# 
# The examples in the table above are from pre-existing designations.  A look
# at the  "Second Dictionary of Nomenclature"  reveals that  unique  2-letter 
# combinations for  acronyms are nearly exhausted. That is the reason for the
# change in the rule for new acronyms where at least three characters are now
# required.  
# Note that "R^136" is a pre-existing  designation,  and therefore it  is not
# altered when creating the designation for a subcomponent even though"R^136"
# does not conform to the rules for creating a new acronym.
# 
# 
# 3.5.2 Examples of improper designations
# 
# 	BD^4deg14 	use of "deg symbol", declination sign missing
#  
# 	N221		no space, unclear source : NGC or N in LMC ?
#   
# 	DLB^J204+2 	leading zero missing; poor position 
# 
# 	P^43578		one letter acronym is ambiguous 
#  
# 	RC^0401+0456 	missing flag letter J for Julian 2000 equatorial 
# 			coordinates, corrected to RC^J0401+0456 in an erratum 
#    
#    
# 4. Advice on designations
# 
# Advice on specific problems may be obtained from representatives of the 
# "Clearing house", a subset of the Task Group on Designations of IAU
# Commission 5: 
# 
# H. R. Dickel
#    Astronomy Dept. Univ. of Illinois, 1002 W. Green Street, Urbana, IL
#    61801-3000, USA  
#    Internet: lanie@astro.uiuc.edu 
#    Phone (217) 244-7044  Fax (217) 244-7638
#  
# P. Dubois
#    Observatoire de Strasbourg 11, rue de l'Universiti F-67000 Strasbourg,
#    FRANCE 
#    Internet: dubois@simbad.u-strasbg.fr 
#    Phone (33) 88-35-84-37  Fax (33) 88-25-01-60 
#    Telex  890506 Code Starobs  NSI/DECnet SIMBAD::DUBOIS
# 
# W. H. Warren Jr
#    Laboratory for Astronomy and Solar Physics, Code 681 NASA Goddard Space
#    Flight Center Greenbelt, MD 20771, USA
#    Internet: w3whw@gibbs.gsfc.nasa.gov 
#    Phone (301) 286-5419  Fax (301) 286-1753
#    NSI/DECnet STARS:WARREN
#  
# M.-C. Lortet 
#    Observatoire de Paris, 25 place Janssen, F-92195 Meudon Cedex, FRANCE     
#    Internet: lortet@mesiob.obspm.fr    
#    Phone (33) 1 4507-7414  Fax (33) 1 4507-7469
#    NSI/DECnet MESIOB::LORTET
# 
# S. Borde
#    Observatoire de Paris, 61 avenue de l'Observatoire,F-75014 Paris, FRANCE 
#    Phone (33) 1 4051-2238  Fax (33) 1 4354-1804
#    Internet: borde@memaga.obspm.fr
# 
# J. M. Dickey
#    Univ. of Minnesota Dept. of Astron., 116 Church St. SE Minneapolis, MN
#    55455 USA 
#    Internet: john@ast1.spa.umn.edu 
#    Phone (612) 624-2895  Fax (612) 626-2029 
# 
# H. J. Andernach
#    IUE Observatory, Villafranca
#    Apartado 50727, E-28080 Madrid, FRANCE
#    Internet: heja@vilspa.esa.es
#    Phone (34) 1-8131-110/102  FAX (34) 1-8131-139/119
# 
# 
# 5. Further information
# 
# For general information, in particular about existing designations, consult
# the following references : 
# 
# Lortet, M.-C., Borde, S., Ochsenbein, F. 1994, The Second Reference
#    Dictionary of the Nomenclature of Celestial Objects, A&AS 107, 193 
# 
#    > The complete paper edition appeared as Publication Speciale du C.D.S.
#      24 Volumes I and II. Observatoire Astronomique de Strasbourg. 
# 
#    > Postscript, LaTex or dvi versions available from CDS via anonymous
#      ftp at the Internet node cdsarc.u-strasbg.fr in the directory /pub/dic
#      following the procedure described in the Editorial note in A&A 280
#      E1-E2 Annual Index 1993
#  
#    > The On-line Dictionary is updated regularly and is available on the
#      free info account installed on the Internet node 
#      simbad.u-strasbg.fr (130.79.128.4) or NSI/DECnet node SIMBAD
#      (18099=17.691). Login as "info"; no password is required. 
# 
#    > A World-Wide-Web Mosaic access to the "On-line" version is under
#      development; access will be announced in the home pages of the 
#      Centre de Donnies de Strasbourg (CDS) at the URL address:
#      http://cdsweb.u-strasbg.fr/CDS.html 
# 
# Fernandez, A., Lortet, M.-C., Spite, F. 1983, The first Dictionary of the
#    Nomenclature of Celestial Objects, A&AS, 52, No 4 
# 
# Lortet, M.-C., Spite, F. 1986, First Supplement to the First Dictionary of
#    the Nomenclature of Celestial Objects, A&AS 64, 329 
# 
# Dickel, H. R., Lortet M.-C., de Boer, K. S. 1987, Designation and
#    Nomenclature for Diffuse Radiating Sources , A&AS, 68, 75
#  
# Jaschek C. 1989, Data in Astronomy, Cambridge University Press 
# 
# 
# (END OF FILE)
# ...........................................................................
X1,f|D|A,0:0:0,0:0:0,99
