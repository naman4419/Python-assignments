def frequency(text):
    words = text.split()
    freq_dict = {}
    
    for word in words:
        word = word.lower()
        if word in freq_dict:
            freq_dict[word] += 1
        else:
            freq_dict[word] = 1
    
    return dict(sorted(freq_dict.items()))

input_text = "mango apple banana apple mango apple"
result = frequency(input_text)
print("Word Frequency:", result)
