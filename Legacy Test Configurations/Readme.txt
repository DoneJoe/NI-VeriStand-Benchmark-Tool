INside this folder are the test system definitions used in the 2009 and 2010 verion of this benchmarker, but upgraded to be usable in 2011. The reason they are legacy is this:
1. Model was compiled without SSE2 enabled
2. Model was compiled with optimization's off
3. DAQ Devices use 16 AI and 2 AO, which most of our cards either have 8 AI and 2 AO or 16 AI and 4 AO
4. Generator's section has 10 generators, which in 2011... you shouldn't need at all unless you're using the legacy profiles

They are kept here for posterity and comparison purposes between versions. However, for maximum performance, don't use these. Use the system definitions in the other folder(s).