# week4.py
READ AND WRITE CHALLENGE

def modify_content(line):
    return line.upper()
def read_and_modify_file(input_filename,output_filename):
    try:
    with open(input_filename,'r')as infile,open(output_filename,'w')as outfile:
    for line in infile:
    modified_line=modify_content(line)
    outfile.write(modified_line)
    print(f"modified content written to {'output-filename'}")
    except FileNotFoundError:
    print(f"file'{input=filename'}not found.")
    Except Exception as e:
    print(f"An error occured"):{"e"}

    ERROR HANDLING LAB

    def read_file():
    FileName=input("Enter the file name:")
    try:
   with open (fileName,'r')as file:
   content=file,read() 
   print("file content:/n")
   print(content)
   except fileNotFoundError:
   print(F"Error:The file'{filenName}'does not exist.")
   Except permission Error:
   print(F"Error:you do not have permission to read'{fileName'.}")
   Except Exception as e:
   print(F"An unexpected error occured:{e}")
