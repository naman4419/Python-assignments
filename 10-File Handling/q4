import os    
import shutil  


source_file = "Users\sriva\Downloads\APPLICATIONS_OF_SECOND-ORDER_DIFFERENTIA (1).pdf"  # This is where the file is now


new_folder = 'new'  


if not os.path.exists(new_folder):
    os.mkdir(new_folder)  
    print("New folder created:", new_folder)
else:
    print("Folder already exists:", new_folder)


destination_file = new_folder + "Users\sriva\Downloads\APPLICATIONS_OF_SECOND-ORDER_DIFFERENTIA (1).pdf"

try:
    shutil.copy(source_file, destination_file)
    print("File copied successfully!")
except FileNotFoundError:
    print("The file you're trying to copy does not exist.")
except Exception as error:
    print("Something went wrong:", error)
