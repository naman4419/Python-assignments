
try:
    with open('file1.txt', 'r') as f1, open('file2.txt', 'r') as f2:
        
        lines1 = f1.readlines()
        lines2 = f2.readlines()

    
    with open('merged.txt', 'w') as output:
        
        max_len = max(len(lines1), len(lines2))

        
        for i in range(max_len):
            if i < len(lines1):
                output.write(lines1[i].rstrip() + '\n')
            if i < len(lines2):
                output.write(lines2[i].rstrip() + '\n')

    print("Files merged successfully into 'merged.txt'.")

except FileNotFoundError as e:
    print("Error: One of the input files was not found.")
    print(e)
except Exception as e:
    print("An error occurred:", e)
