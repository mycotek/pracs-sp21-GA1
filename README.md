# This is a respository for my assignment
## About the repository
This respository contains information about the Illinois Mycological Association including my personal experiences and links to get more information. 
## The code used to rename the sample data files
I used a `for` loop to rename the file extensions on the sample data files from .txt to .csv.
```
for sample in *.txt
do
newname=$(basename "$sample" .txt).csv
echo "Old/new name: $sample $newname"
mv "$sample" "$newname"
done
```