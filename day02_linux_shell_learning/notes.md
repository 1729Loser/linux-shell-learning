touch file1.txt #created the file1.txt
touch f1.txt f2.txt #updated/changed the f2.txt file timestamp taking reference from f1.txt
touch -d "2020-01-01 12:00:00" file ==>  0 Jan  1  2020 file #the timestamp of the file changed/updated to given timestamp
touch -t 202501012359 file ==> 0 Jan  1  2025 file #the timestamp of the file updated/changed 

input ==> file f1.txt
output ==> f1.txt: ASCII text
input ==>  file -b compressed.tar
output ==> POSIX tar archive (GNU)
input ==> file -i secondscript.sh
output ==> secondscript.sh: text/x-shellscript; charset=us-ascii
input ==> file -f f1.txt 
output ==> "doing what you love is most beautifull thing": cannot open `"doing what you love is most beautifull thing"' (No such file or directory)
jai.jpg:                                        ASCII text

input ==> cat f2.txt
output ==> " it is never too late for a new beginning in your life "
           " you don't have to be great to start, but you have to start to be great "
           " bravery is measured by how hard you try, not by whether you actually succeed "
input ==> cat f3.txt f2.txt
output ==>  " ఇసుమంత ఆచరణ , ఇరవై వేల టన్నుల వ్యర్థమైన మాటలతో సమానం "
            " it is never too late for a new beginning in your life "
            " you don't have to be great to start, but you have to start to be great "
            " bravery is measured by how hard you try, not by whether you actually succeed "
input ==> cat > newfile.txt
" never trust your fears, they don't know your strength "
" every day is a fresh start, a blank canvas to paint upon "
output ==> cat newfile.txt
            " never trust your fears, they don't know your strength "
            " every day is a fresh start, a blank canvas to paint upon "

less f2.txt ==> it displays f2.txt file content in less viewer

history ==> displays all the list of commands we used
history -c ==> deletes the list of commands which are present in history
history -d 3==> deletes the particular 3 keynote command in the history list
