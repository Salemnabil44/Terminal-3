1/ grep -i "PHP" wilders.csv | grep -i "France" | grep "2019" | wc -l > php_france_2019.csv
cat php_france_2019.csv 

2/ 
(création des fichiers demandés) touch javascript_biarritz_toulouse.csv wilders.csv php_france_2019.csv 

(premier filtre Toulouse + Biarritz, la fonction -i rend permet de faire une recherche sans faire de distinction entre majuscules et minuscules lors de la recherche.) 
grep -i "JavaScript" wilders.csv | grep -i "Toulouse" > javascript_toulouse.csv
   
(deuxième filtre Biarritz + JavaScript) grep -i "JavaScript" wilders.csv | grep -i "Biarritz" > javascript_biarritz.csv  
  
(concaténer) cat javascript_biarritz.csv javascript_toulouse.csv >javascript_toulouse_biarritz.csv 
  
(résultat) cat javascript_toulouse_biarritz.csv 
