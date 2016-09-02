### Count the number of items in a comma seperated row
```
echo "0,2,4,0,1,2,4,5,0,4,6,3,0,1,0" | tr , '\n' | wc -l
```
