# !. How can I run saffron tree with Docker

1.
   ```
    docker pull sangerpathogens/saffrontree
   ```
   
2.
  ```
   mkdir saffron-data
  ```

3.
  ```
   git clone https://github.com/sanger-pathogens/saffrontree.git
  ```
  
4. 
  ```
    cp saffrontree/saffrontree/example_data/fastqs/* saffron-data/
  ```
  
5.
 ```
   docker run --rm -it -v `pwd`/saffron-data:/data sangerpathogens/saffrontree saffrontree output start_Salmonella_enterica_subsp_enterica_serovar_Paratyphi_A_str_AKU_12601_v2_1.fastq.gz
 ```
