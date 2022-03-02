# Example submission directory for grid-control jobs

Submission on lxplus via to condor simply proceeds via:

`go.py skimmer_condor.conf`

Note that you need to update the location of your X509_USER_PROXY in the configuration file, and clearly also the SE path to write to and the CMSSW project area

### Rucio hack

grid-control temporarily did not support rucio, which required for each sample to obtain a list of filenames with the `read_filelist_from_das.py` script, and then to add the produced txt file to the dataset via the `list:` argument.

Note that this hack may not be needed anymore since there were updates to grid-control, but I haven't tested it yet
