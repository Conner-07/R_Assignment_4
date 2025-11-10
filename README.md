# R_Assignment_4

This R script reads the DNA sequence file that I downloaded in the first assignment called chr1_GL383518v1_alt.fa. It prints specific bases from the sequence, builds the reverse complement, and then counts how many A, C, G, and T bases are in each 1kb section of the sequence. Everything was done using base R without any extra packages.

To run the script, open R and set the working directory to the folder that has the FASTA file and my R file using setwd("/Users/connerstarkey/Informatics_573"). Then run source("Assignment4.R"). When it runs, it prints the sequence length, the 10th and 758th bases, the 79th base of the reverse complement, and the bases from 500 to 800. After that it builds a table showing the base counts per kilobase.

The files included are Assignment4.R which is my main script, chr1_GL383518v1_alt.fa which is the sequence I used, and data_summary.txt which was made automatically by the shell script.

For the questions, the expected sum for each list is 1000 because each kilobase section should have 1000 total bases (A + C + G + T). A few of the lists don’t equal 1000. This happens because the last section is shorter than 1kb and also because any positions that have N, which means an unknown base, are not counted in the totals. The differences are just from those two reasons, and otherwise the totals add up correctly.
