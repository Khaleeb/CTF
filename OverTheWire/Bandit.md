# Over the Wire: Wargames

*Notes:*
- bandit.labs.overthewire.org
- port 2220

## Level 0
ssh -p 2220 bandit0@bandit.labs.overthewire.org  

## Level 0->1

cat readme:  
    NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL  

## Level 1->2

cat ./- :  
    rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi

## Level 2->3

cat spaces\ in\ this\ filename :  
    aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG

## Level 3->4

cat inhere/.hidden :  
    2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe

## Level 4->5

file inhere/* ;  
cat inhere/-file07 :  
    lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR


## Level 5->6

ls -Rla inhere/ | grep 1033  
cat inhere/maybehere07/.file2  
    P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU


## Level 6->7

find . -size 33c -group 11006 -user 11007 2>/dev/null  
    z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S

## Level 7->8

cat data.txt | grep "millionth"  
    TESKZC0XvTetK0S9xNwm25STk5iWrBvP

## Level 8->9

cat data.txt | sort | uniq -u  
    EN632PlfYiZbn3PhVK3XOGSlNInNE00t

## Level 9->10

cat data.txt | strings | grep "==="  
    G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s

## Level 10->11

cat data.txt  | base64 -d  
    6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM

## Level 11->12

cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'  
    JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv

## Level 12->13

*xxd -r to reverse hexdump to bin, use file to see top-level compression*  
xxd -r | gunzip | bunzip2 | gunzip | tar | tar |  bunzip2 | tar | gunzip  
    wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw

## Level 13->14

