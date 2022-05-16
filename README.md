there are three main files listed
seedgen.py              group-95 nine
Rseed.py                ld98 is working on
filehash.py             janeSero3 is working on making it work

generated file that should be encrypted 'seedgen.txt' and singed with the partial hash from the sha256

seedgen.py --a--> seedgen.txt --b--> Rseed.py
       \                  /__________/
        \_______________/
         |
         ^--c--> filehash.py --c--> #? saltedchain
                                                |
         BLOCKCHAIN/DASYCHAIN <-----------------/

defenitions:
(a) have the out put file example on lines 11 through 15

## seedRX is appended to seedgen.txt for now
f=open("E://lens_v0.0.1-main/seedgen.txt","a")
f.writelines("\n")
f.writelines(seedRX)
f.close()

(b) reading the file using the Rseed.py

(c) have the file to be hashed
hashing the seedgen.py and salting with the Rseed.py to put into the hypothetical saldedchain
to lock the file from being edited 

