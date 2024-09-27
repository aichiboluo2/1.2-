# 1.2 当堂作业
## 1）
```
cd /home/test/linux
cd ~/linux
gunzip 1.gtf.gz
ls  
```
`1.gtf  file`
```

`cat 1.gtf | head  #显示1.gtf文件前10行`
```
IV      ensembl gene    1802    2953    .       +       . gene_id "YDL248W"; gene_version "1"; gene_name "COS7"; gene_source "ensembl"; gene_biotype "protein_coding";
IV      ensembl transcript      1802    2953    .       + .     gene_id "YDL248W"; gene_version "1"; transcript_id "YDL248W"; transcript_version "1"; gene_name "COS7"; gene_source "ensembl"; gene_biotype "protein_coding"; transcript_name "COS7"; transcript_source "ensembl"; transcript_biotype "protein_coding";
IV      ensembl exon    1802    2953    .       +       . gene_id "YDL248W"; gene_version "1"; transcript_id "YDL248W"; transcript_version "1"; exon_number "1"; gene_name "COS7"; gene_source "ensembl"; gene_biotype "protein_coding"; transcript_name "COS7"; transcript_source "ensembl"; transcript_biotype "protein_coding"; exon_id "YDL248W.1"; exon_version "1";
IV      ensembl CDS     1802    2950    .       +       0 gene_id "YDL248W"; gene_version "1"; transcript_id "YDL248W"; transcript_version "1"; exon_number "1"; gene_name "COS7"; gene_source "ensembl"; gene_biotype "protein_coding"; transcript_name "COS7"; transcript_source "ensembl"; transcript_biotype "protein_coding"; protein_id "YDL248W"; protein_version "1";
IV      ensembl start_codon     1802    1804    .       + 0     gene_id "YDL248W"; gene_version "1"; transcript_id "YDL248W"; transcript_version "1"; exon_number "1"; gene_name "COS7"; gene_source "ensembl"; gene_biotype "protein_coding"; transcript_name "COS7"; transcript_source "ensembl"; transcript_biotype "protein_coding";
```
`cat 1.gtf | tail  #显示1.gtf文件后10行`


```
Mito    ensembl exon    85035   85112   .       +       . gene_id "tM(CAU)Q2"; gene_version "1"; transcript_id "tM(CAU)Q2"; transcript_version "1"; exon_number "1"; gene_source "ensembl"; gene_biotype "tRNA"; transcript_name "tM(CAU)Q2"; transcript_source "ensembl"; transcript_biotype "tRNA"; exon_id "tM(CAU)Q2.1"; exon_version "1";
Mito    ensembl gene    85295   85777   .       +       . gene_id "RPM1"; gene_version "1"; gene_source "ensembl"; gene_biotype "ncRNA";
Mito    ensembl transcript      85295   85777   .       + .     gene_id "RPM1"; gene_version "1"; transcript_id "RPM1"; transcript_version "1"; gene_source "ensembl"; gene_biotype "ncRNA"; transcript_name "RPM1"; transcript_source "ensembl"; transcript_biotype "ncRNA";
Mito    ensembl exon    85295   85777   .       +       . gene_id "RPM1"; gene_version "1"; transcript_id "RPM1"; transcript_version "1"; exon_number "1"; gene_source "ensembl"; gene_biotype "ncRNA"; transcript_name "RPM1"; transcript_source "ensembl"; transcript_biotype "ncRNA"; exon_id "RPM1.1"; exon_version "1";
Mito    ensembl gene    85554   85709   .       +       . gene_id "Q0297"; gene_version "1"; gene_source "ensembl"; gene_biotype "protein_coding";
Mito    ensembl transcript      85554   85709   .       + .     gene_id "Q0297"; gene_version "1"; transcript_id "Q0297"; transcript_version "1"; gene_source "ensembl"; gene_biotype "protein_coding"; transcript_name "Q0297"; transcript_source "ensembl"; transcript_biotype "protein_coding";
Mito    ensembl exon    85554   85709   .       +       . gene_id "Q0297"; gene_version "1"; transcript_id "Q0297"; transcript_version "1"; exon_number "1"; gene_source "ensembl"; gene_biotype "protein_coding"; transcript_name "Q0297"; transcript_source "ensembl"; transcript_biotype "protein_coding"; exon_id "Q0297.1"; exon_version "1";
Mito    ensembl CDS     85554   85706   .       +       0 gene_id "Q0297"; gene_version "1"; transcript_id "Q0297"; transcript_version "1"; exon_number "1"; gene_source "ensembl"; gene_biotype "protein_coding"; transcript_name "Q0297"; transcript_source "ensembl"; transcript_biotype "protein_coding"; protein_id "Q0297"; protein_version "1";
Mito    ensembl start_codon     85554   85556   .       + 0     gene_id "Q0297"; gene_version "1"; transcript_id "Q0297"; transcript_version "1"; exon_number "1"; gene_source "ensembl"; gene_biotype "protein_coding"; transcript_name "Q0297"; transcript_source "ensembl"; transcript_biotype "protein_coding";
Mito    ensembl stop_codon      85707   85709   .       + 0     gene_id "Q0297"; gene_version "1"; transcript_id "Q0297"; transcript_version "1"; exon_number "1"; gene_source "ensembl"; gene_biotype "protein_coding"; transcript_name "Q0297"; transcript_source "ensembl"; transcript_biotype "protein_coding";
```

`cat 1.gtf | head -15  #显示1.gtf文件前15行(输入值15可以用其他整数替代)`
`ls -lh 1.gtf  #显示1.gtf文件的大小`
`wc -l 1.gtf  #统计1.gtf文件行数`


`grep -v "^#" 1.gtf | grep -v '^$' | wc -l `


`cat 1.gtf | awk '$0!~/^\s*$/{print}' | head -10`
`grep -v '^\s*$' 1.gtf | head -10`
