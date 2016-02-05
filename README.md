# BREW

This simple utility aimed to convert illumina fastq files into a single sqlite3 database for following processing.
```bash
>>> python brew.py -o some.db file1.fastq@table1 file2.fastq@table2 ... file_n.fastq@table_n 
```

It also have a dry-run option ```-d```, which is convenient for test runs
```bash
>>> python brew.py -o some.db /home/magniff/Downloads/seqs/{r1.fastq@forward,r2.fastq@reverse,barcode.fastq@barcode} -d
Processing file '/home/magniff/Downloads/seqs/r1.fastq' into table 'forward'
Processing file '/home/magniff/Downloads/seqs/r2.fastq' into table 'reverse'
Processing file '/home/magniff/Downloads/seqs/barcode.fastq' into table 'barcode'

```
