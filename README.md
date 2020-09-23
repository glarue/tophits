usage: tophits [-h] [-n NUMBER_OF_HITS] [-e E_VALUE_CUTOFF] [-d] [-s] [-m]
               [-r]
               blast_file

Reports the top n BLAST hits for each query in a (tabular) blast output file

positional arguments:
  blast_file

optional arguments:
  -h, --help            show this help message and exit
  -n NUMBER_OF_HITS, --number_of_hits NUMBER_OF_HITS
                        number of hits to report for each unique query
                        (default: 1)
  -e E_VALUE_CUTOFF, --e_value_cutoff E_VALUE_CUTOFF
                        exclude hits with e-value greater than this value
                        (default: None)
  -d, --allow_duplicate_target_hits
                        allow multiple hits to the same subject to be included
                        (default: False)
  -s, --sort_by_name    sort output by name rather than bitscore (default:
                        False)
  -m, --memory_efficient
                        avoid reading entire dataset into memory at once, to
                        increase memory efficiency (default: False)
  -r, --redundant_ids   allow query and subject to share the same identifier
                        (default: False)
