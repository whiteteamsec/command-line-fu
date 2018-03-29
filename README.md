# Bash command line fu:

List out all the emails recursively from root and save it in text file <br />
grep -E -o -r "[A-Za-z0-9][A-Za-z0-9._%+-]+@[A-Za-z0-9][A-Za-z0-9.-]+\.[A-Za-z]{2,6}"  /root/ > save.txt

Extract email address only from file <br />
grep -o '[[:alnum:]+\.\_\-]*@[[:alnum:]+\.\_\-]*' save.txt | sort | uniq –I 

