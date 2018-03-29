# Bash command line fu:

List out all the emails recursively from root and save it in text file
grep -E -o -r "[A-Za-z0-9][A-Za-z0-9._%+-]+@[A-Za-z0-9][A-Za-z0-9.-]+\.[A-Za-z]{2,6}"  /root/ > save.txt

Extract email address only from file
grep -o '[[:alnum:]+\.\_\-]*@[[:alnum:]+\.\_\-]*' save.txt | sort | uniq –I 

