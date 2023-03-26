# SAGERoute: Synergistic Analog Routing Considering Geometric and Electrical Constraints with Manual Design Compatibility

## Overview
SAGERoute takes circuit netlist, technology file and user defined config as input to generate the high-quality solution for analog circuit. 

![](figs/fig.png)

## Test 
```
./paprika/main/sageroute \ 
--techfile="../benchmark/mockPDK/lef.json"  \
--paramfile="../benchmark/ota2/config.json" \ 
--netlist="../benchmark/ota2/ota2.sp"       \
--placement="../benchmark/ota2/ota2.json"   \
--constraints="../benchmark/ota2/elec.json" \
--result="../benchmark/ota2/ota2.gds"         
```


## Contact

For any questions, please do not hesitate to contact us.

```
Haoyi Zhang: hy.zhang@stu.pku.edu.cn
```
