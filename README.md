## pymol tools

## Requirements

- pymol

## Alpahfold colouring

https://kpwulab.com/2023/03/09/color-alphafold2s-plddt/

'''
spectrum b, red_yellow_green_cyan_blue, minimum=50, maximum=90

set_color n0, [0.051, 0.341, 0.827]
set_color n1, [0.416, 0.796, 0.945]
set_color n2, [0.996, 0.851, 0.212]
set_color n3, [0.992, 0.490, 0.302]
color n0, b < 100; color n1, b < 90
color n2, b < 70;  color n3, b < 50

spectrum b, rainbow_rev, minimum=0, maximum=100
'''

OR 
run https://raw.githubusercontent.com/cbalbin-bio/pymol-color-alphafold/master/coloraf.py

coloraf model_name

## for ray tracing

on the 2nd structure
set ray_trace_mode,1
set ray_trace_color, black
ray 600,600
set ray_opaque_background, off

copy the structure to new obj
select obj
show surface
set transparency, 0.6

png /path/to/folder/ex.png, dpi=1000


## Contributing

DEHourigan
 
## Contact

For any queries, please reach out via GitHub issues or directly to `114402828@umail.icc.ie`.

---
