# Project structure

Input/output files for EasyDiffraction are in simple and human-readable data format STAR/CIF with the specifications of [International Union of Crystallography](https://www.iucr.org), where possible.

Example project structure for the constant wavelength powder neutron diffraction measurement is given below:

```
La0.5Ba0.5CoO3     - Project directory.
├── project.cif    - Main project description file.
├── models         - Folder with individual crystallographic phases.
│   ├── lbco.cif   - File with La0.5Ba0.5CoO3 phase parameters.
│   └── ...
├── experiments    - Folder with instrumental parameters and measured data.
│   ├── hrpt.cif   - Measured data from HRPT@PSI & instrumental parameters.
│   └── ...
└── summary
    └── report.cif - Summary report after structure refinement.
```

Here is the content of the project files:

### project.cif

```c++
data_La0.5Ba0.5CoO3

_description "neutrons, powder, constant wavelength, HRPT@PSI"

loop_
_model_cif_file_name
lbco.cif

loop_
_experiment_cif_file_name
hrpt.cif
```

### models / lbco.cif

```c++
data_lbco

_space_group_name_H-M_alt "P m -3 m"
_space_group_IT_coordinate_system_code 1

_cell_length_a      3.8909(1)
_cell_length_b      3.8909
_cell_length_c      3.8909
_cell_angle_alpha  90
_cell_angle_beta   90
_cell_angle_gamma  90

loop_
_atom_site_label
_atom_site_type_symbol
_atom_site_fract_x
_atom_site_fract_y
_atom_site_fract_z
_atom_site_occupancy
_atom_site_adp_type
_atom_site_B_iso_or_equiv
_atom_site_multiplicity
_atom_site_Wyckoff_symbol
La La   0   0   0     0.5  Biso 0.4958   1 a
Ba Ba   0   0   0     0.5  Biso 0.4943   1 a
Co Co   0.5 0.5 0.5   1    Biso 0.2567   1 b
O  O    0   0.5 0.5   1    Biso 1.4041   3 c
```

### experiments / hrpt.cif

```c++
data_hrpt

_diffrn_radiation_probe neutron
_diffrn_radiation_wavelength 1.494

_pd_meas_2theta_offset  0.6225(4)

_pd_instr_resolution_u  0.0834
_pd_instr_resolution_v -0.1168
_pd_instr_resolution_w  0.123
_pd_instr_resolution_x  0
_pd_instr_resolution_y  0.0797

_pd_instr_reflex_asymmetry_p1 0
_pd_instr_reflex_asymmetry_p2 0
_pd_instr_reflex_asymmetry_p3 0
_pd_instr_reflex_asymmetry_p4 0

loop_
_phase_label
_phase_scale
lbco 9.0976(3)

loop_
_pd_background_2theta
_pd_background_intensity
10  174.3
20  159.8
30  167.9
50  166.1
70  172.3
90  171.1
110 172.4
130 182.5
150 173.0
165 171.1

loop_
_pd_meas_2theta
_pd_meas_intensity
_pd_meas_intensity_sigma
10     167 12.6
10.05  157 12.5
10.1   187 13.3
10.15  197 14
10.2   164 12.5
10.25  171 13
...
164.6  153 20.7
164.65 173 30.1
164.7  187 27.9
164.75 175 38.2
164.8  168 30.9
164.85 109 41.2
```
