# SAGERoute: Synergistic Analog Routing Considering Geometric and Electrical Constraints with Manual Design Compatibility

## Overview
SAGERoute takes circuit netlist, technology file and user defined config as input to generate the high-quality solution for analog circuit. 

![](Overview.png)

## Introduction of the input
```
techfile:    Basic information of technology lib. Here we release a mock PDK for your test
paramfile:   Some parameters for user to directly control the routing kernel 
netlist:     A formal netlist generated from CDF file
placement:   Here we only release the placement generated by automatic tools(coord only format). The manual placement(gds format) can't be realeased due to the NDA
constraints: The electric current information of the circuit
result:      You could save the gds result here
```
## Compilation Platform
```
Operating system:  Ubuntu 18.04 
GCC version:  7.5.0
Runtime dependency: GCC 7.5.0, Lpsolve
```

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


## Citation section

```
@inproceedings{chen2023macrorank,
    author = {Zhang, Haoyi and Gao, Xiaohan and Luo, Haoyang and Song, Jiahao and Liu, Junhua and Tang, Xiyuan and Lin, Yibo and Wang, Runsheng and Huang, Ru},
    title = {SAGERoute: Synergistic Analog Routing Considering Geometric and Electrical Constraints with Manual Design Compatibility},
    year = {2023},
    numpages = {6},
    location = {Antwerp, Belgium},
    series = {DATE '23}
}
```

## Contact

For any questions, please do not hesitate to contact us or raise issues on Github.

```
Haoyi Zhang: hy.zhang@stu.pku.edu.cn
```
