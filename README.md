# sprint 1a
# 1) 123 rəqəmini string/character-ə çevirin və tipini yoxlayın
num = 123
string_num = str(num)
print(string_num, type(string_num))

# 2) 19.99 dəyərini tam ədədə çevirin və nəticəni çap edin
value = 19.99
int_value = int(value)
print(int_value)

# 3) "500" dəyərini numeric-ə çevirin və 2-yə bölüb nəticəni çap edin
text_num = "500"
numeric_value = int(text_num)
print(numeric_value / 2)

# 4) a = 8 və b = 12 yaradın. a < b və a == b şərtlərini yoxlayın, nəticələri çap edin
a = 8
b = 12
print("a < b:", a < b)
print("a == b:", a == b)

# 5) x = 5, y = 10, z = 15 yaradın. (x < y) and (y < z) şərtini yoxlayın və nəticəni çap edin
x = 5
y = 10
z = 15
print("(x < y) and (y < z):", (x < y) and (y < z))

# 6) 25-i 4-ə bölün. Tam bölmə, qalıq və adi bölmə nəticələrini çap edin
print("Tam bölmə:", 25 // 4)
print("Qalıq:", 25 % 4)
print("Adi bölmə:", 25 / 4)

# 7) 3-ü 4-cü dərəcəyə qaldırın və nəticəni çap edin
print("3^4 =", 3 ** 4)

# 8) qiymet = 75.5 yaradın. Onu tam ədədə çevirin və tipini yoxlayın
qiymet = 75.5
qiymet_int = int(qiymet)
print(qiymet_int, type(qiymet_int))

# 9) n = 20 yaradın. (n > 10) or (n < 5) və (n > 15) and (n < 25) şərtlərini yoxlayın, nəticələri çap edin
n = 20
print("(n > 10) or (n < 5):", (n > 10) or (n < 5))
print("(n > 15) and (n < 25):", (n > 15) and (n < 25))

# 10) "42.8" dəyərini əvvəl float-a, sonra tam ədədə çevirin və hər addımda tipi yoxlayın
val = "42.8"
float_val = float(val)
print(float_val, type(float_val))
int_val = int(float_val)
print(int_val, type(int_val))

#sprint_1b
# 1) s = "Programming" yaradın. Uzunluğunu və ilk simvolunu çap edin
s = "Programming"
print("Uzunluq:", len(s))
print("İlk simvol:", s[0])

# 2) s1 = "Hello" və s2 = "World" yaradın. Onları boşluqla birləşdirin və nəticəni çap edin
s1 = "Hello"
s2 = "World"
print(s1 + " " + s2)

# 3) text = "Python" yaradın. Son simvolunu çap edin
text = "Python"
print("Son simvol:", text[-1])

# 4) s = "Artificial" yaradın. "Art" hissəsini ilə çıxarın və çap edin
s = "Artificial"
print(s[3:])  # "Art" = s[0:3], s[3:] qalan hissə

# 5) word = "Code" yaradın. Tərsinə çevirin və nəticəni çap edin
word = "Code"
print(word[::-1])

# 6) s = "abcdefgh" yaradın. Hər ikinci simvolu alın və çap edin
s = "abcdefgh"
print(s[::2])

# 7) text = "data" yaradın. Onu bir sətrlik kodla böyük və kiçik hərflərə çevirib çap edin
text = "data"
print(text.upper(), text.lower())

# 8) s = "Python-R-Java" yaradın. "-" ilə ayırın və nəticəni çap edin
s = "Python-R-Java"
print(s.split("-"))

# 9) ad = "Ayxan" və yaş = 25 yaradın. f-string ilə "Ayxan 25 yaşındadır" çap edin
ad = "Ayxan"
yaş = 25
print(f"{ad} {yaş} yaşındadır")

# 10) s = "salam-dunya" yaradın. "-"ni boşluqla əvəz edin və nəticəni çap edin
s = "salam-dunya"
print(s.replace("-", " "))

#sprint_2a
# 1) 
numbers = [5, 10, 15, 20]

# 2) 
print("Length:", len(numbers))

# 3) 
numbers.append(25)
print("After adding 25:", numbers)

# 4) 
numbers.insert(2, 12)
print("After inserting 12 at index 2:", numbers)

# 5) 
list1 = [1, 2, 3]
list2 = [4, 5, 6]
merged = list1 + list2
print("Merged list:", merged)

# 6) 
print("2nd and 3rd elements:", numbers[2:4])

# 7) 
numbers[0] = 50
print("First element replaced with 50:", numbers)

# 8) 
print("Is 19 in the list?", 19 in numbers)

# 9) 
letters = ["a", "b", "a", "c"]
print('Number of "a":', letters.count("a"))

# 10) 
chars = ["x", "y", "x", "z"]
chars = [c for c in chars if c != "x"]
print('After removing "x":', chars)

# 11) 
nums = [7, 2, 9, 1]
nums.sort(reverse=True)
print("Sorted in descending order:", nums)
12)
greater_than_10 = [n for n in numbers if n > 10]
print("Elements greater than 10:", greater_than_10)

#sprint_2b
import pandas as pd

# 1) 
s1 = pd.Series([10, 20, 30, 40])

# 2) 
s1.index = ['w', 'x', 'y', 'z']
print("s1:\n", s1)

# 3) 
s2 = pd.Series({'p': 5, 'q': 10, 'r': 15})
print("s2:\n", s2)

# 4) 
print("Element with index 'q':", s2['q'])

# 5) 
print("s1 elements > 25:\n", s1[s1 > 25])

# 6)
print("s1 elements > 20 divided by 10:\n", s1[s1 > 20] / 10)

# 7) 
df1 = pd.DataFrame([(1, 2), (3, 4)])

# 8) 
df1.index = ['r1', 'r2']
df1.columns = ['c1', 'c2']
print("df1:\n", df1)

# 9) 
df2 = pd.DataFrame({'A': [1, 2], 'B': [3, 4]})
print("df2:\n", df2)

# 10) 
print("Rows where column 'A' > 1:\n", df2[df2['A'] > 1])
