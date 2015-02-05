# LTRANS
My modification of LTRANS v.2 to cater our own application.

The original LTRANS was obtained from http://northweb.hpl.umces.edu/LTRANS.htm

Modifications include:
* In my forcing files the variables Cs_r, Cs_w, s_rho, and s_w are recorded as global attributes rather than regular variables. I attempt to modify LTRANS to read them in.

* Detect the length of unlimited dimension to support variable number of time frames in the nc forcing files.

* Read each forcing file only up to 2nd last time frame to avoid reading in duplicate forcing records. 
