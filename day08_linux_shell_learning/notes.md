# read.txt
  jai
  sree
  ram
  jai
  sree
  ram

  when we use uniq command for this file it prints exact same thing without removing repeated lines.
  because it is not sorted .
  after sorting the file and with the help of pipe(|) when we use uniq command then it prints only one line for every repeated line and rest non repeated lines it prints that same line only
 
  # sort read.txt | uniq
      the output will be like this
      jai
      sree
      ram

# grep is versatile and powerful tool in linux environment.
    The true power of grep is unlocked when you combine it with other commands using pipes (|).
    This allows us to filter the output of any command.

# that's it for today.
