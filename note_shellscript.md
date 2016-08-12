#!/bin/bash

# 配列の各要素を参照 ${配列名[インデックス]}
# 配列の全要素参照 ${配列名[@]}
# 配列の要素数を参照 ${#配列名[*]}


# if$BJ8$N;H$$J}(B
read -p "Please Enter Your Age : " age

if [ $age -ge 20 ] ; then
  echo "You can Drink"
else
  echo "You can NOT Drink"
fi


# for$BJ8$N;H$$J}(B
read -a char_array -p "Please Enter 3 Literature : "

for i in ${char_array[@]} 
do
  echo $i
done

# while$B$N;H$$J}(B
# select$B$N;H$$J}(B
#select name in "apple" "banana" "orange"
#do
#  echo "You selected $name";
#done

# while$B$N;H$$J}(B
# while$B$N;H$$J}(B
# while$B$N;H$$J}(B
while true
do
  echo "Continue? (y/n)"
  read input
  case $input in
    n) break
      ;;
    y) continue
      ;;
    *) echo "Please input y or n ."
      ;;
    esac
done
