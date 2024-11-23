def sort_string(input_string):
    lowercase = []
    uppercase = []
    digits = []
    special_chars = []

    for char in input_string:
        if char.islower():
            lowercase.append(char)
        elif char.isupper():
            uppercase.append(char)
        elif char.isdigit():
            digits.append(char)
        else:
            special_chars.append(char)


    lowercase.sort()
    uppercase.sort()
    digits.sort()
    special_chars.sort()


    sorted_string = ''.join(digits + lowercase + uppercase + special_chars)

    return sorted_string



input_string = input("یک رشته وارد کنید: ")
# چاپ خروجی
print(sort_string(input_string))
