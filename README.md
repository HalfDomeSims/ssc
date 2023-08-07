# ssc

Data accopmanying paper: [Super-sample covariance of the power spectrum, bispectrum, halos, voids, and their cross-covariances](https://arxiv.org/abs/2210.15647)

We provide the local and global overdensity (delta) grids for cdm and halos in the following location:. 

Please contact Adrian Bayer <abayer@princeton.edu> for any additional data.

# Filename definitions

In all below cases, color is an integer between 0 and 511 which labels the sub-boxes, seed is an integer between 0 and 511 which labels the small boxes and SU boxes, and lg is a string 'l' or 'g' denoting the local or global mesh respectively.

## Sub-boxes
### cdm
'proc4096_nc2048_size5000_nsteps60lin_ldr0_rcvfalse_fstnone_pnf2_lnf2_s100_pgdfalse_fll0.20/subbox/z0/cdm/color%d/stats/delta_%s_Nmesh256_c1i0cic.npy' % (color, lg)

### fof
'proc4096_nc2048_size5000_nsteps60lin_ldr0_rcvfalse_fstnone_pnf2_lnf2_s100_pgdfalse_fll0.20/subbox/z0/fof/color%d/stats/N/delta_%s_Nmesh256_c1i0cic_Nmin80.npy % (color, lg)

## Small boxes:
### cdm
'proc64_nc256_size625_nsteps60lin_ldr0_rcvfalse_fstnone_pnf2_lnf2_s%d_pgdfalse_fll0.20/subbox/z0/cdm/color0/stats/delta_l_Nmesh256_c1i0cic.npy' % (1000 + seed)

### fof
'proc64_nc256_size625_nsteps60lin_ldr0_rcvfalse_fstnone_pnf2_lnf2_s%d_pgdfalse_fll0.20/subbox/z0/fof/color0/stats/N/delta_l_Nmesh256_c1i0cic_Nmin80.npy' % (1000 + seed)

## SU
### fid

#### cdm
'proc64_nc256_size625_nsteps60lin_ldr0_rcvtrue_fstnone_pnf2_lnf2_s%d_pgdfalse_fll0.20_ODE/subbox/z0/cdm/color0/stats/delta_l_Nmesh256_c1i0cic.npy' % (1000 + seed)

#### fof
'proc64_nc256_size625_nsteps60lin_ldr0_rcvtrue_fstnone_pnf2_lnf2_s%d_pgdfalse_fll0.20_ODE/subbox/z0/fof/color0/stats/N/delta_l_Nmesh256_c1i0cic_Nmin80.npy' % (1000 + seed)

### -delta_b

#### cdm
'proc64_nc256_size631_nsteps60lin_ldr0_rcvtrue_fstnone_pnf2_lnf2_s1000_pgdfalse_fll0.20_ODE_su_db-3.000e-02/subbox/z0/cdm/color0/stats/delta_l_Nmesh256_c1i0cic.npy' % (1000 + seed)

#### fof
'proc64_nc256_size631_nsteps60lin_ldr0_rcvtrue_fstnone_pnf2_lnf2_s1000_pgdfalse_fll0.20_ODE_su_db-3.000e-02/subbox/z0/fof/color0/stats/N/delta_l_Nmesh256_c1i0cic_Nmin80.npy' % (1000 + seed)

### +delta_b
#### cdm
'proc64_nc256_size619_nsteps60lin_ldr0_rcvtrue_fstnone_pnf2_lnf2_s1000_pgdfalse_fll0.20_ODE_su_db3.000e-02/subbox/z0/cdm/color0/stats/delta_l_Nmesh256_c1i0cic.npy' % (1000 + seed)

#### fof
'proc64_nc256_size619_nsteps60lin_ldr0_rcvtrue_fstnone_pnf2_lnf2_s1000_pgdfalse_fll0.20_ODE_su_db3.000e-02/subbox/z0/fof/color0/stats/N/delta_l_Nmesh256_c1i0cic_Nmin80.npy' % (1000 + seed)
