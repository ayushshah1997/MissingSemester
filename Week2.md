1. ls -a -h -t -l
2. 
```
marco() {
    dir=$(pwd)
}

polo() {
    cd "$dir"
}
```
3. 
```
i=0
rm log.txt
while :
do 
    i=$((i+1))
    ./aa.sh >> log.txt
    if [ "$?" -eq 1 ]; then
        echo "i is $i"
        cat log.txt
        exit 1
    fi
done
```
4. 
```
find -name '*.html' | xargs zip a.zip
```