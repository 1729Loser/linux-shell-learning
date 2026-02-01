cp f1.txt /home/matrix/Documents #f1.txt is coped to Documents directory
input ==>  cp *.txt /home/thematrix/Desktop
output ==> bashcmds.txt  f1.txt  f2.txt  f3.txt  file1.txt  newfile.txt #the all files with .txt extension are coped to Desktop directory

input ==> cp f[0-9].t?? /home/thematrix/Projects #all the in between 0-9 numbers contained files starting with the name f and extenstion starting with .t and after that there may be any letters betweeen [a-Z] should be coped to Project directory
output ==> f1.txt  f2.txt  f3.txt #and here those files

input ==>  cp -r Projects/ /home/matrix/Pictures
output ==> Pictures/Projects:
           f1.txt  f2.txt  f3.txt
           
input ==>  cp -i f1.txt /home/thematrix/Videos
output ==> cp: overwrite '/home/thematrix/Videos/f1.txt'? #it asks permission to overwrite the f1.txt file which is already exist in Videos directory. after giving persmission it copies the file

input ==> cp -f f1.txt /home/thematrix/Videos
output ==> # it doesn't asks for permission to overwrite

input ==>  cp -p f1.txt /home/matrix/3
output ==> # it replicates it's all content and it's metadata from original one




mv oldfilename newfilename #renaming oldfilename to newfilename
mv file /xdirectory #moving file to the xdirectory
mv file1 file2 /ydirectory #at a time moving file1 & file2 to the ydirectory 
input ==> mv -t /adirectory f1 f2 f3 f4 f5 
output ==> #it used to many files at a time but first giving destination location then after mentions files which we want to move. which is gives as a clear cut view

input ==> mv -i f*.txt /home/matrix/3
output ==>mv: overwrite '/home/matrix/3/f1.txt'?   #it asks persmission to overwrite the files
          mv: overwrite '/home/matrix/3/f2.txt'?
          mv: overwrite '/home/matrix/3/f3.txt'?
          mv: overwrite '/home/matrix/3/file1.txt'?
          
input ==> mv -b f1.txt /home/matrix/3
output ==> f1.txt  f1.txt~ # it keeps the old file renaming it with a tilde (~) suffix

input ==>  mv -v f1.txt /home/matrix/
output ==> renamed 'f1.txt' -> '/home/matrix/f1.txt' # it shows what does command mv is doing. here it is renaming the file



mkdir matrix
mkdir doc proj vid #creating mutliple directories at a time
input ==> mkdir -p home/matrix/git
output ==> # created nested directories. home as main directory with a subdirectory matrix with subsubdirectory git. if any one of the directories are not present. if home directory present as main then it creates nested directories from matrix

input ==> mkdir -m 700 privatefolder
output ==> # creating a directory with mode (nothing but giving permissions who can do and what can able to do )




rm file.txt #removed the file.txt file
input ==> rm -i file
output ==> rm: remove regular empty file 'file'? yes #asks permission before deleting the file named file

input ==> rm -ir Projects #every time asks permission before deleting any file and directory
output ==> rm: descend into directory 'Projects'? yes 
           rm: remove regular file 'Projects/f2.txt'? yes
           rm: remove regular file 'Projects/f3.txt'? yes
           rm: remove directory 'Projects'? no

input ==> rm -f file1.txt
output ==> # it doesn't permission to remove, forcefully it will delete any file or directory

input ==>  rm -r Pictures/ 
output ==> # it is used to remove the subdirectories, content and files of the Pictures directory

input ==> rm -d Documents/ or rmdir Documents/
output ==> # both are used to delete the empty directory
