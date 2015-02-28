# Language Identification and Transliteration (LIT): 

This tool is used for language identification and transliteration of Indic-words in code-mixed data. 

The tool is meant for seven Indian languages; Hindi, Bengali, Kanadda, Tamil, Malayalam and Gujrati code mixed with English. 

The input file should contain text in only two languages, English and any of the above mentioned Indian languages. 

It is necessary to mention the Indian language used in the code-mixed data by passing an argument after the input file as shown below. 

## Requirements:

    kenlm. Can be installed from 'https://github.com/kpu/kenlm'
    numpy. Can be installed via 'sudo apt-get install python-numpy'

## Preprocessing:

    1.  Unzip all files in blm_models directory using the following command:

	    gunzip blm_models/*

    2.  Move to convertor-indic-1.4.9 directory and copy its path using pwd command to the .bashrc file as shown below:

	    export convertorIndic="path"    
	    e.g.
	    export convertorIndic="/home/irshad/LIT/convertor-indic-1.4.9"    


### How to use ??

    python lang_idf_tran.py -f inputfile -t hin|ban|kan|mal|tam|guj|tel -o[optional] T

    Third argument -o is optional. Set the argument to T to skip transliteration\


Contact :

Irshad Ahmad Bhat

MS-CSE IIITH, Hyderabad

bhatirshad127@gmail.com

irshad.bhat@research.iiit.ac.in
