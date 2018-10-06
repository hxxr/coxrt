## Test environments
* R 3.5.1 (2017-01-27); Platform: x86_64-pc-linux-gnu (64-bit); Running under: Ubuntu 14.04.5 LTS (on travis-ci) 
* R 3.5.1 (2018-07-02); Platform: x86_64-w64-mingw32 (64-bit) (local Windows computer)

## R CMD check results
On both platforms there were no ERRORs or WARNINGs. 

In Windows there was 1 NOTE:
* checking compiled code ... NOTE File 'coxrt/libs/x64/coxrt.dll': Found no calls to: 'R_registerRoutines', 'R_useDynamicSymbols'

Explanation: I use 'useDynLib(coxrt, .registration = TRUE)' in NAMESPACE file, but for some reason it does not remove this NOTE.


