# Inequity-Aversion-Pricing
Data File (zip) for Extended graph formulation for the inequity aversion pricing problem (written by Chopra, Park and Shim)
Please refer to 
https://www.researchgate.net/publication/346300880_Extended_Graph_Formulation_for_the_Inequity_Aversion_Pricing_Problem_on_Social_Networks?channel=doi&linkId=5fbdab7b92851c933f57b20e&showFulltext=true


This data repository contains a python code to solve the inequity aversion pricing problem on social network data used in the following article:
"Extended graph formulation for the inequity aversion pricing problem" (written by Chopra, Park and Shim)


<inequityAversionPricing.py>

Lines 7 - 8 read 'lines_[datanum].csv' file in 'lines' folder and read 'nodes_[datanum]_[repnum].csv' file in 'nodes' folder
Line 7: datanum = 0 # Data ID 0 - 9
Line 8: repnum = 0 # Replicate ID : Random Value Function

Lines 14 - 16 set the discount options (activate only one line)
Line 14: priceOptions = ['discontinuity', 200, 400, 500] # Table 1
Line 15: # priceOptions = ['discontinuity', 66, 88, 101, 148, 210, 317, 416, 435, 536] # Table 2
Line 16: # priceOptions = ['discontinuity', 30, 60, 90, 120, 150, 180, 210, 240, 270, 300, 330, 360, 390, 420, 450, 480, 510, 540, 570, 600] # Table 3

Lines 18 - 20 set the tolerance (activate only one line)
Line 18: tolerance = 100 # Table 1
Line 19: # tolerance = 75 # Table 2
Line 20: # tolerance = 0 # Table 3


<Data: 'lines_[datanum].csv' files in 'lines' folder>
Each file has 3 columns: 'Line', 'Source', 'Target'. Column 'Line' is the line ID. Each line is a friend relationship between two friends 'Source' and 'Target'.


<Data: 'nodes_[datanum]_[repnum].csv' files in 'nodes' folder>
Each file has two columns: 'Node', 'Value'. Column 'Node' is the user ID. The value of the product to the user is written in Column 'Value'.
