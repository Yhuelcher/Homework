## Homework 06/07/2015

 **1. Using Chipotle looking at the head and tail. Look how the data is structured. What does each column mean? Looking at more file content.**
 
  ```cd ~/desktop/dat7/data```
  
  ```head chipotle.tsv```
  
  ```tail chipotle.tsv```
  
  ```head -n20 chipotle.tsv```

  ```tail -n20 chipotle.tsv```

It appears to be a tab delimited file with columns and rows. The columns give back the oderid, how many items, the item itself and the description of the item as well as the price. 


**2. How many orders appear in the file?**

        1834

**3. How many lines are in the file?**


  ```wc -l chipotle.tsv```
  
        4623


**4. Which burrito is more popular steak burrito or chicken burrito?**

  ```grep -i 'steak burrito' chipotle.tsv | wc -l```
  
        *368*

  
  ```grep -i 'chicken burrito' chipotle.tsv | wc -l```
  
        *553*

chicken is more popular than steak


**5. Do chicken have more often Pinto Beans over Black Beans**

  ```grep -i 'chicken burrito' chipotle.txt > burrito.txt```
  
    ```grep -i 'pinto beans' burrito.txt | wc -l```
        105


    ```grep -i 'black beans' burrito.txt | wc -l```
        282

Black beans are used more often

**6. Make a list of all cvs and tsv files**

  ```find data *.csv *.tsv```
  
        airlines.csv
        
        chipotle.tsv
        
        sms.tsv 

**7. Number of occurance of the word 'dictionary' within all files of dat7.**

  ```grep -ir 'dictionary'.| wc -w```


