# cgcnn_with_dielectric
## INTRODUCTION:
Hello all,
- Here we have added dielectric constant as a feature in Crystal Graph Convolutional Neural Network (CGCNN), so that we can try improving the prediction of the property: Band Gap.
- We have done extracted data  from Materials Project database and JARVIS database and found that the e_electronic(electronic component of Band Gap) shows an inverse trend with Band gap.

## How to use this:
- The initial structure remains the same as using CGCNN, make your own custom dataset, add your CIF files,id_prop.csv and atom_init.json files. Now also add a file named DE.csv.
- DE.csv should contain the one hot encoded vector of the dielectric feature for each CIF-ID with a precise length of 4.
- We have tried binning the dielectric constants in 0-5,5-10,10-15,15+.
- You can choose your own ranges of bins as long as the length of the one hot encoded vector remains 4.

## CONCLUSION:
- After that is done, train and test using the normal queries of CGCNN.

### THANK YOU!


