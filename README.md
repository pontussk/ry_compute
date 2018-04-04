# ry_compute
Inferring the biological sex of ancient genomic shotgun samples

# Example usage: 
samtools view <MYBAM.bam> | python ry_compute.py [options] 

Options:
  -h, --help            show this help message and exit
  --chrXname=CHRXNAME   Identifier for the X chromosome in the SAM input (use
                        if different than chrX, X etc)
  --chrYname=CHRYNAME   Identifier for the Y chromosome in the SAM input (use
                        if different than chrY, Y etc)
  --malelimit=MALELIMIT
                        Upper R_y limit for assignment as XY/male
  --femalelimit=FEMALELIMIT
                        Lower R_y limit for assignment as XX/female
  --digits=DIGITS       Number of decimal digits in R_y output
  --noheader            Do not print header describing the columns in the
                        output
  --idxstats            Input is from samtools idxstats
