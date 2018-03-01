Meghan O'Leary

The regulatory constraints incorporate the boolean rules used by Palsson

Assumptions:
The lower bound for the anaerobic case without regulatory constraints was set to -0.0001 for M_o2_e since
a lower bound of 0 resulted in no growth.

Following metabolites and reactions were "on" for the regulatory constraint cases:

M_o2_e=1 (aerobic) and 0 (anerobic)

M_succ_e=1;

M_fum_e=1;

M_mal_L_e=1;

M_glc_D_e=1;

M_ac_e=1;

M_nh4_e=1;

M_pi_e=1;

M_lac_D_e=1;

M_fru_e=1;

R_ME2=1;

R_ME1=1;

R_GLCpts=1;

R_PYK=1;

R_PFK=1;

R_LDH_D=1;

R_SUCCt2_2=1;

M_glu_L_e=1;

Following reactions were "off" for the regulatory constraint cases:

R_FBP=0;

R_TKT2=0;

R_TALA=0;

R_PGI=0;

Running the code:
1. Open "Solve.jl" to edit
2. Comment out loading of data_dictionary for all but the one you wish to solve.
3. Save changes made
4. cd into the source file in Julia/command prompt
5. In julia type include("Solve.jl") and hit enter
6. When julia has finished solving type flux_array[24] to get the flux value for that specific case
7. Repeat for all 4 cases

Results:

Aerobic without regulatory constraints: 0.09166474637510488 / hr

Anaerobic without regulatory constraints: 5.308137374595246e-5 / hr

Aerobic with regulatory constraints: 0.04142665672795142 / hr

Anaerobic with regulatory constraints: 0.02742681360490633 / hr
