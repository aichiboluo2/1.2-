# 1.2 当堂作业
## step0
```
cd /home/test/linux
cd ~/linux
gunzip 1.gtf.gz
ls  
```
`1.gtf  file`
## step1

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
```
IV      ensembl gene    1802    2953    .       +       . gene_id "YDL248W"; gene_version "1"; gene_name "COS7"; gene_source "ensembl"; gene_biotype "protein_coding";
IV      ensembl transcript      1802    2953    .       + .     gene_id "YDL248W"; gene_version "1"; transcript_id "YDL248W"; transcript_version "1"; gene_name "COS7"; gene_source "ensembl"; gene_biotype "protein_coding"; transcript_name "COS7"; transcript_source "ensembl"; transcript_biotype "protein_coding";
IV      ensembl exon    1802    2953    .       +       . gene_id "YDL248W"; gene_version "1"; transcript_id "YDL248W"; transcript_version "1"; exon_number "1"; gene_name "COS7"; gene_source "ensembl"; gene_biotype "protein_coding"; transcript_name "COS7"; transcript_source "ensembl"; transcript_biotype "protein_coding"; exon_id "YDL248W.1"; exon_version "1";
IV      ensembl CDS     1802    2950    .       +       0 gene_id "YDL248W"; gene_version "1"; transcript_id "YDL248W"; transcript_version "1"; exon_number "1"; gene_name "COS7"; gene_source "ensembl"; gene_biotype "protein_coding"; transcript_name "COS7"; transcript_source "ensembl"; transcript_biotype "protein_coding"; protein_id "YDL248W"; protein_version "1";
IV      ensembl start_codon     1802    1804    .       + 0     gene_id "YDL248W"; gene_version "1"; transcript_id "YDL248W"; transcript_version "1"; exon_number "1"; gene_name "COS7"; gene_source "ensembl"; gene_biotype "protein_coding"; transcript_name "COS7"; transcript_source "ensembl"; transcript_biotype "protein_coding";
IV      ensembl stop_codon      2951    2953    .       + 0     gene_id "YDL248W"; gene_version "1"; transcript_id "YDL248W"; transcript_version "1"; exon_number "1"; gene_name "COS7"; gene_source "ensembl"; gene_biotype "protein_coding"; transcript_name "COS7"; transcript_source "ensembl"; transcript_biotype "protein_coding";
IV      ensembl gene    3762    3836    .       +       . gene_id "YDL247W-A"; gene_version "1"; gene_source "ensembl"; gene_biotype "protein_coding";
IV      ensembl transcript      3762    3836    .       + .     gene_id "YDL247W-A"; gene_version "1"; transcript_id "YDL247W-A"; transcript_version "1"; gene_source "ensembl"; gene_biotype "protein_coding"; transcript_name "YDL247W-A"; transcript_source "ensembl"; transcript_biotype "protein_coding";
IV      ensembl exon    3762    3836    .       +       . gene_id "YDL247W-A"; gene_version "1"; transcript_id "YDL247W-A"; transcript_version "1"; exon_number "1"; gene_source "ensembl"; gene_biotype "protein_coding"; transcript_name "YDL247W-A"; transcript_source "ensembl"; transcript_biotype "protein_coding"; exon_id "YDL247W-A.1"; exon_version "1";
IV      ensembl CDS     3762    3833    .       +       0 gene_id "YDL247W-A"; gene_version "1"; transcript_id "YDL247W-A"; transcript_version "1"; exon_number "1"; gene_source "ensembl"; gene_biotype "protein_coding"; transcript_name "YDL247W-A"; transcript_source "ensembl"; transcript_biotype "protein_coding"; protein_id "YDL247W-A"; protein_version "1";
```


`ls -lh 1.gtf  #显示1.gtf文件的大小`<br>
`-rw-rw-r-- 1 test test 12M Sep 11  2018 1.gtf`<br>

`wc -l 1.gtf  #统计1.gtf文件行数`<br>
`42252 1.gtf`<br>

`grep -v "^#" 1.gtf | grep -v '^$' | wc -l `<br>
`42247`<br>

`cat 1.gtf | awk '$0!~/^\s*$/{print}' | head -10`<br>
```
IV      ensembl gene    1802    2953    .       +       . gene_id "YDL248W"; gene_version "1"; gene_name "COS7"; gene_source "ensembl"; gene_biotype "protein_coding";
IV      ensembl transcript      1802    2953    .       + .     gene_id "YDL248W"; gene_version "1"; transcript_id "YDL248W"; transcript_version "1"; gene_name "COS7"; gene_source "ensembl"; gene_biotype "protein_coding"; transcript_name "COS7"; transcript_source "ensembl"; transcript_biotype "protein_coding";
IV      ensembl exon    1802    2953    .       +       . gene_id "YDL248W"; gene_version "1"; transcript_id "YDL248W"; transcript_version "1"; exon_number "1"; gene_name "COS7"; gene_source "ensembl"; gene_biotype "protein_coding"; transcript_name "COS7"; transcript_source "ensembl"; transcript_biotype "protein_coding"; exon_id "YDL248W.1"; exon_version "1";
IV      ensembl CDS     1802    2950    .       +       0 gene_id "YDL248W"; gene_version "1"; transcript_id "YDL248W"; transcript_version "1"; exon_number "1"; gene_name "COS7"; gene_source "ensembl"; gene_biotype "protein_coding"; transcript_name "COS7"; transcript_source "ensembl"; transcript_biotype "protein_coding"; protein_id "YDL248W"; protein_version "1";
IV      ensembl start_codon     1802    1804    .       + 0     gene_id "YDL248W"; gene_version "1"; transcript_id "YDL248W"; transcript_version "1"; exon_number "1"; gene_name "COS7"; gene_source "ensembl"; gene_biotype "protein_coding"; transcript_name "COS7"; transcript_source "ensembl"; transcript_biotype "protein_coding";<br>
```

`grep -v '^\s*$' 1.gtf | head -10`

```
IV      ensembl gene    1802    2953    .       +       . gene_id "YDL248W"; gene_version "1"; gene_name "COS7"; gene_source "ensembl"; gene_biotype "protein_coding";
IV      ensembl transcript      1802    2953    .       + .     gene_id "YDL248W"; gene_version "1"; transcript_id "YDL248W"; transcript_version "1"; gene_name "COS7"; gene_source "ensembl"; gene_biotype "protein_coding"; transcript_name "COS7"; transcript_source "ensembl"; transcript_biotype "protein_coding";
IV      ensembl exon    1802    2953    .       +       . gene_id "YDL248W"; gene_version "1"; transcript_id "YDL248W"; transcript_version "1"; exon_number "1"; gene_name "COS7"; gene_source "ensembl"; gene_biotype "protein_coding"; transcript_name "COS7"; transcript_source "ensembl"; transcript_biotype "protein_coding"; exon_id "YDL248W.1"; exon_version "1";
IV      ensembl CDS     1802    2950    .       +       0 gene_id "YDL248W"; gene_version "1"; transcript_id "YDL248W"; transcript_version "1"; exon_number "1"; gene_name "COS7"; gene_source "ensembl"; gene_biotype "protein_coding"; transcript_name "COS7"; transcript_source "ensembl"; transcript_biotype "protein_coding"; protein_id "YDL248W"; protein_version "1";
IV      ensembl start_codon     1802    1804    .       + 0     gene_id "YDL248W"; gene_version "1"; transcript_id "YDL248W"; transcript_version "1"; exon_number "1"; gene_name "COS7"; gene_source "ensembl"; gene_biotype "protein_coding"; transcript_name "COS7"; transcript_source "ensembl"; transcript_biotype "protein_coding";<br>
```

## step2
### step2.1:选取1-3列的数据（以下两种命令都可以）

`cat 1.gtf | awk ' { print $1, $2, $3 } ' | head`<br>
```
IV ensembl gene
IV ensembl transcript
IV ensembl exon
IV ensembl CDS
IV ensembl start_codon
```

`cat 1.gtf | cut -f 1,2,3 | head`
```
IV      ensembl gene
IV      ensembl transcript
IV      ensembl exon
IV      ensembl CDS
IV      ensembl start_codon
```

### step 2.2

`cat 1.gtf | awk '$3 =="gene" { print $1, $3, $9 } ' | head`
```
IV gene gene_id
IV gene gene_id
IV gene gene_id
IV gene gene_id
IV gene gene_id
IV gene gene_id
IV gene gene_id
IV gene gene_id
IV gene gene_id
IV gene gene_id
```
## step3.提取和计算特定的feature
### step3.1 提取并统计featrue类型
`grep -v '^#' 1.gtf |awk '{print $3}'| sort | uniq -c`  #提取并计数有多少类feature<br>
```
   7050 CDS
   7553 exon
   7126 gene
   6700 start_codon
   6692 stop_codon
   7126 transcript
```
### step3.2 计算特定feature特征长度

`cat 1.gtf | awk ' { print $3, $5-$4 + 1 } ' | head` 
```
1
 1
 1
 1
 1
gene 1152
transcript 1152
exon 1152
CDS 1149
start_codon 3
```
#计算所有CDS的总长度<br>
```
cat 1.gtf | awk 'BEGIN{size=0;}$3 =="CDS"{ len=$5-$4 + 1; size += len; print "Size:", size } ' | tail -n 1<br>
Size: 9030648
```

#或者用awk只在最后输出统计的结果:
`cat 1.gtf | awk 'BEGIN{L=0;}$3 =="CDS"{L+=$5-$4 + 1;}END{print L;}'`<br>
`9030648`<br>
#或者利用awk自动初始化的特性:<br>
`cat 1.gtf | awk '$3 =="CDS"{L+=$5-$4 + 1;}END{print L;}'`<br>
`9030648`<br>
#计算1号染色体cds的平均长度
#awk既可从pipe中读取输入，也可从文件中读取输入<br>
`awk 'BEGIN  {s = 0;line = 0;}$3 =="CDS" && $1 =="I"{ s += $5-$4+1;line += 1}END {print "mean="s/line}' 1.gtf`<br>
`mean=1239.52`<br>
