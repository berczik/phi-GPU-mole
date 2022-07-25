# phi-GPU-mole
Parallel Hermite Integration on GPU (Direct N-body on MOLE-8.5 cluster)

-----------------------------------------------------------
This is a short readme file for the first public version of 
"phi-GPU" N-body program.

The phi-GPU-mole.tar.gz file contain the exact version of 
code which was used for the large set of test runs on the 
Mole-8.5 GPU cluster of the IPE CAS, Beijing, China 
around April 2011. The results are in the code paper:

https://ui.adsabs.harvard.edu/abs/2011hpc..conf....8B/abstract

-----------------------------------------------------------

This is a fully GPU (and only NVIDIA GPU + CUDA code). We 
start to develop this code together with Keigo Nitadori 
around the end of 2008. 

Basically we fully rewrite our earlier MPI parallel phi-GRAPE 
("C" code) code using the new "C++" standards and CUDA calls. 
The code was written "around" the Keigo Nitadori & Junichiro 
Makino earlier high order (Hermite 4th, 6th & 8th) CPU 
integrator:

- K. Nitadori and J. Makino. Sixth- and eighth-order
  Hermite integrator for N-body simulations. 
  New Astronomy, 13:498-507, Oct. 2008.

The code directly work with the GPU's. No need in any kind 
of external (like SAPPORO) libraries. 

The code is distributed "as is". Please, if you use the code for 
any "productive" or even "test" runs cite our papers: 

-----------------------------------------------------------
Code details in HPC conference:

   https://ui.adsabs.harvard.edu/abs/2011hpc..conf....8B/abstract

   High performance massively parallel direct N-body
   simulations on large GPU clusters.

   Peter Berczik, Keigo Nitadori, Shiyan Zhong, 
   Rainer Spurzem, Tsuyoshi Hamada, Xiaowei Wang
   Ingo Berentzen, Alexander Veles, Wei Ge

   International conference on High Performance Computing,
   Kyiv, Ukraine, October 8-10, 2011.

First large N astrophysical results:

   http://adsabs.harvard.edu/abs/2012ApJ...756...30K

   Formation and Hardening of Supermassive Black Hole 
   Binaries in Minor Mergers of Disk Galaxies.

   Khan Fazeel Mahmood, Berentzen Ingo, Berczik Peter,
   Just Andreas, Mayer Lucio, Nitadori Keigo, Callegari Simone

   The Astrophysical Journal, Volume 756, Issue 1, article 
   id. 30, 10 pp. (2012). 
------------------------------------------------------------

In this papers (especially in the first one) we are in detail 
analize the performance of the different parts of the code.

In any other questions or want to report some problems with the 
code please send me the e-mail or contact me in any other way. 

All the best, Peter Berczik.

*****************************************
Dr.Sci. Peter Berczik

Main Astronomical Observatory
National Academy of Sciences of Ukraine, 
MAO/NASU, 27 Akademika Zabolotnoho St.
03143 Kyiv, Ukraine

E-mail: berczik@mao.kiev.ua
Office: +38 (044) 526-47-71
Mobil:  +38 (099) 503-72-62
Skype1:  berczik-office
Skype2:  berczik (on phone)
*****************************************
