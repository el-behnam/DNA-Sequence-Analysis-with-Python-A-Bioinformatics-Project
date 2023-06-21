# DNA Sequence Analysis Problem

In this problem, your task is to write a Python program that reads a file containing DNA sequences in multi-FASTA format, and compute the answers to the following questions:

## Problem Details

1. **How many records are in the file?**
   - A record in a FASTA file is defined as a single-line header, followed by lines of sequence data. The header line is distinguished from the sequence data by a greater-than (">") symbol in the first column. The word following the ">" symbol is the identifier of the sequence, and the rest of the line is an optional description of the entry. There should be no space between the ">" and the first letter of the identifier. 

2. **What are the lengths of the sequences in the file?**
   - What is the longest sequence and what is the shortest sequence?
   - Is there more than one longest or shortest sequence?
   - What are their identifiers? 

3. **Identify open reading frames (ORFs)**
   - In molecular biology, a reading frame is a way of dividing the DNA sequence of nucleotides into a set of consecutive, non-overlapping triplets (or codons). Depending on where we start, there are six possible reading frames: three in the forward (5' to 3') direction and three in the reverse (3' to 5').
   - An open reading frame (ORF) is the part of a reading frame that has the potential to encode a protein. It starts with a start codon (ATG), and ends with a stop codon (TAA, TAG or TGA).
   - Given an input reading frame on the forward strand (1, 2, or 3) your program should be able to identify all ORFs present in each sequence of the FASTA file, and answer the following questions: 
   - What is the length of the longest ORF in the file?
   - What is the identifier of the sequence containing the longest ORF?
   - For a given sequence identifier, what is the longest ORF contained in the sequence represented by that identifier?
   - What is the starting position of the longest ORF in the sequence that contains it? The position should indicate the character number in the sequence. 

4. **Identify repeats in the DNA sequence**
   - A repeat is a substring of a DNA sequence that occurs in multiple copies (more than one) somewhere in the sequence. Although repeats can occur on both the forward and reverse strands of the DNA sequence, we will only consider repeats on the forward strand here.
   - Also, we will allow repeats to overlap themselves. 
   - Given a length n, your program should be able to identify all repeats of length n in all sequences in the FASTA file.
   - Your program should also determine how many times each repeat occurs in the file, and which is the most frequent repeat of a given length.
you can use 'dna.example.fasta' file for your practice as it is smaller and the 'dna2.fasta' file is for testing how the program works on a real size data.

Remember to return to the main [README](./README.md) file to check how to proceed after understanding this problem.
