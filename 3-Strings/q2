def lowercase(s):
    result = ""
    for char in s:
        if 'A' <= char <= 'Z':
            result += chr(ord(char) + 32)
        else:
            result += char
    return result

def uppercase(s):
    result = ""
    for char in s:
        if 'a' <= char <= 'z':
            result += chr(ord(char) - 32)
        else:
            result += char
    return result

def togglecase(s):
    result = ""
    for char in s:
        if 'a' <= char <= 'z':
            result += chr(ord(char) - 32)  
        elif 'A' <= char <= 'Z':
            result += chr(ord(char) + 32)  
        else:
            result += char
    return result

input = input("Enter a string: ")

print("Lowercase:", lowercase(input))
print("Uppercase:", uppercase(input))
print("Toggle Case:", togglecase(input))
