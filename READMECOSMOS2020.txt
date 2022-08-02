######################## COSMOS2020 masks ########################
This is a description of all the masks in the COSMOS2020 catalogue 
All the detected objects selected with the different flags are shown in
- flags_in_catalog.png

The convention is:
flag = 0   -   the object is GOOD  meaning is outside the masked out area
flag = 1   -   the object is BAD   meaning is inside the masked out area

#=============== HSC bright star masks ===============
Bright stars masks from the HSC survey are provided from

1) HSC PRD2: revised masks from incremental release 1 (2018, https://hsc-release.mtk.nao.ac.jp/doc/index.php/bright-star-masks-2/). Masks are given for g,r,i,z bands and the combined mask for all griz bands

- MASK_HSC-stars_griz_COSMOS2020.reg - updated April 2022, removing exterior frame
	Area of flag=0: 2.850 deg2

	Corresponds to FLAG_HSC

#================ SuprimeCam masks ================
Same mask used in COSMOS2015 - mask from Peter

- MASK_SUPCAM_COSMOS2020.reg - updated April 2022, removing exterior frame
	Area of flag=0: 1.833 deg2  
	
	Corresponds to FLAG_SUPCAM

#================ UltraVista region mask ==============
Borders of UltraVista layout in images 4 rectangles, above, below, left and right.

- MASK_UVISTA_COSMOS2020.reg
	Area of flag=0: 1.792 deg2  
	
	Corresponds to FLAG_UVISTA

#================ UltraDeep stripes = ==============
Regions of the UltraDeep stripes inside the UltraVista field

- MASK_UDEEP_COSMOS2020.reg
	Area of flag=0: 1.057 deg2
	
	Corresponds to FLAG_UDEEP

#=====Notes=====
All the masked out areas are computed within a rectangle of 
-RA_min  149.058  -RA_max  151.064 
-DEC_min 1.391    -DEC_max 3.072
With an area of 3.37 deg2
This is the area in which objects are detected in the CLASSIC catalog

The area selected by FLAG_COMBINED = 0 is 1.278 deg2

