try:
    with open('source.txt', 'r') as source_file:
        
        content = source_file.read()

        
        content_upper = content.upper()

        
        with open('destination.txt', 'w') as destination_file:
            destination_file.write(content_upper)

        print("File copied successfully with lowercase letters changed to uppercase.")

except FileNotFoundError:
    print("Error: 'source.txt' not found.")
except Exception as e:
    print("An error occurred:", e)
