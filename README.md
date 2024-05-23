# Details

This is an f statistic calculator for generated fake spectra. The `.xcm` file only serves as an example. User `.xcm` loaded data will be different. The `xcm` file consists of `tcl` script that loops over the fake data and calculates the f statistic using the fake spectra and the original spectra. The number of fake spectra can be adjusted from the `.xcm` loop. 
This sort of a script was employed for calculating the posterior predictive p-value using the `fakeit` command in *xspec*
In general, the script can be modified to caculate and other statistic other than the f-statistic. This will be automated eventually.

## Instructions:

- Copy the `calc-f-stat.sh` and the `f-stat.xcm` files to the location containing the all fake spectra files and the fake background files. The location must also contain the original `.fits` spectrum file, `.fits` background file and the `.rmf` response file.
- Make the `.sh` file executable by opening a terminal and entering the following command
  
  > ```console
  > chmod u+x calc-f-stat.sh
  > ```
- Execute using `./calc-f-stat.sh`
- An output file named `f_statistic.txt` will be generated which will contain all the f statistic values.
