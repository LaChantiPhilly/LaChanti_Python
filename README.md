LaChanti_Python

****__PYTHON FUNDAMENTALS_****

# Any python interperter can be used as a calculator:
3 + 5 * 4
    23
# Lets save a value to a variable
weight_kg = 60
print(weight_kg) 60

# Weight0 = valid
# 0weight = invalid
# weight and Weight are different
# Types of data 
# There are three common types of data
# Interger numbers
# floating point numbers 
# Strings
# Floating point number**

weight_kg = 60.3
# String comprised of Letters
patient_name = "Jon Smith"
# String comprised of numbers
patient_id = '001'

# Use variables in python

weight_lb = 2.2 * weight_kg

print(weight_lb)
    132.66

# lets add a prefix to our patient id 

patient_id = 'inflam_' + patient_id

print(patient_id)

    inflam_001

# Lets combine print statements

print(patient_id, 'weight in likograms:', weight_kg)

    inflam_001 weight in likograms: 60.3

# we can call a function inside another function

print(type(60.3))

print(type(patient_id))

    <class 'float'>
    <class 'str'>

# We can also do calculations inside the print function

print('weight in lbs:', 2.2 * weight_kg)

    weight in lbs: 132.66

print(weight_kg)
    60.3
weight_kg = 65.0
print('weight in kilograms is now', weight_kg)

    weight in kilograms is now 65.0






******_STORING VALUES IN LIST-PYTHON_****__**__

odds = [1, 3, 5, 7,]
print('odds are:', odds)

 odds are: [1, 3, 5, 7]

print('first element:', odds[0])
print('last element', odds[3])
print('"-1" element', odds[-1])

    first element: 1
    last element 7
    "-1" element 7

names = ['Curie', 'Darwing', 'Turing'] # Typo in Darwin's name
print('names is orginally:', names)
names[1] = 'Darwin' # Correct the name
print('final value of names:', names)
    names is orginally: ['Curie', 'Darwing', 'Turing']
    final value of names: ['Curie', 'Darwin', 'Turing']
#name= 'Darwin'
#name[0] = 'd'
odds.append(11)
print('odds after adding a value:', odds)

    odds after adding a value: [1, 3, 5, 7, 11]
removed_element = odds.pop(0)
print('odds after removing the first element:', odds)
print('removed_element:', removed_element)

    odds after removing the first element: [3, 5, 7, 11]
    removed_element: 1
odds.reverse()
print('odds after reversing:', odds)

    odds after reversing: [11, 7, 5, 3]

odds = [3,5,7]
primes = odds
primes.append(2)
print('primes:', primes)
print('odds:', odds)

    primes: [3, 5, 7, 2]
    odds: [3, 5, 7, 2]

odds = [3,5,7]
primes = list(odds)
primes.append(2)
print('primes:', primes)
print('odds:',odds)

    primes: [3, 5, 7, 2]
    odds: [3, 5, 7]

binomial_name = "Drosophila melaanogaster"
group = binomial_name[0:10]
print('group:', group)

species = binomial_name[11:23]
print('species:', species)

chromosomes = ['X', 'Y', '2', '3', '4']
autosomes = chromosomes[2:5]
print('autosomes:', autosomes)

last = chromosomes[-1]
print('last:', last)

    group: Drosophila
    species: melaanogaste
    autosomes: ['2', '3', '4']
    last: 4

date = 'Monday 4 January 2023'
day = date[0:6]
print('Using 0 to begin range:', day)
day = date[:6]
print('Omitting beginning index:', day)

    Using 0 to begin range: Monday
    Omitting beginning index: Monday

months = ['jan', 'feb', 'mar', 'apr', 'may', 'jun', 'jul', 'aug', 'sep', 'oct', 'nov', 'dec']
sond = months[8:12]
print('With known last position:', sond)

sond = months[8:len(months)]
print('Using len() to get last entry:', sond)

sond = months[8:]
print('Omitting ending index:', sond)


    With known last position: ['sep', 'oct', 'nov', 'dec']
    Using len() to get last entry: ['sep', 'oct', 'nov', 'dec']
    Omitting ending index: ['sep', 'oct', 'nov', 'dec']





**_ USING LOOPS_**

odds = [1,3,5,7]

print(odds[0])
print(odds[1])
print(odds[2])
print(odds[3])

    1,3,5,7

odds = [1,3,5]
print(odds[0])
print(odds[1])
print(odds[2])
print(odds[3])
 
    1,3,5

odds = [1, 3, 5, 7, 9, 11, 13, 15, 17, 19]

for num in odds:
    print(num)
1,3,5,7,9,11,13,15,17,19

length = 0
names = ['Curie', 'Darwin', 'Turing']
for value in names:
    length = length + 1
print('There are', length, 'names in the list.')

    There are 3 names in the list.

name = "Rosalind"
for name in ['Curie', 'Darwin', 'Turing']:
    print(name)
print('after the loop, name is', name)
   
    Curie
    Darwin
    Turing
    after the loop, name is Turing


print(len([0, 1, 2, 3]))
  4

name = ['Curie', 'Darwin', 'Turing']

print(len(name))
 3







***_MAKING CHOICES_***

num = 37
if num > 100:
    print('greater')
else:
    print('not greater')
print('done')

    not greater
    done

num = 53
print('before conditional...')
if num > 100:
    print(num, 'is greater than 100')
print('...after conditional')

    before conditional...
    ...after conditional

num = 14
if num > 0:
    print(num, 'is  positive')
elif num == 0:
    print(num, 'is zero')
else:
    print(num, 'is negative')

    14 is  positive

if (1 > 0) and (-1 >= 0):
    print('both parts are true')
else:
    print('atleast one part is false')

    atleast one part is false

if (1 > 0) or (-1 >= 0):
    print('at least one part is true')
else:
    print('both of these are false')

    at least one part is true






***_FUNCTIONS 1_***

fahrenheit_val = 99
celsius_val = ((fahrenheit_val - 32) *(5/9))

print(celsius_val)
```

    37.22222222222222

fahrenheit_val2 = 43
celsius_val2 = ((fahrenheit_val2 -32) *(5/9))

print(celsius_val2)

    6.111111111111112

def explicit_fahr_to_celsius(temp):
    # Assign the converted value to a variable
    converted = ((temp - 32) * (5/9))
    # Return the values of the new variable
    return converted

def fahr_to_celsius(temp):
    # Return converted values more effeciently using the return function without creating
    # a new variable. This code does the same thing as the previous function but it is more
    # explicit in explaining how the return command works.
    return ((temp - 32) * (5/9))

fahr_to_celsius(32)
 0.0

explicit_fahr_to_celsius(32) 
0.0

print('Freezing point of water:', fahr_to_celsius(32), 'C')
print('Boiling point of water:', fahr_to_celsius(212), 'C')


    Freezing point of water: 0.0 C
    Boiling point of water: 100.0 C

def celsius_to_kelvin(temp_c):
    return temp_c + 273.15

print('freezing point of water in Kelvin:', celsius_to_kelvin(0.))
     freezing point of water in Kelvin: 273.15

def fahr_to_kelvin(temp_f):
    temp_c = fahr_to_celsius(temp_f)
    temp_k = celsius_to_kelvin(temp_c)
    return temp_k

print('freezing point of water in Kelvin:', fahr_to_kelvin(212.0))
    freezing point of water in Kelvin: 373.15

temp_kelvin = fahr_to_kelvin(212.0)
print('Temperature in Kelvin was:', temp_kelvin)

    Temperature in Kelvin was: 373.15

temp_kelvin: 373.15

def print_temperatures():
    print('Temperature in Fahrenheit was:', temp_fahr)
    print('Temperature in Kelvin was:', temp_kelvin)
    
temp_fahr = 212.0
temp_kelvin = fahr_to_kelvin(temp_fahr)

print_temperatures()

    Temperature in Fahrenheit was: 212.0
    Temperature in Kelvin was: 373.15





***_DEFENSIVE PROGRAMMING_***

numbers = [1.5, 2.3, 0.7, -0.001, 4.4]
total = 0.0
for num in numbers:
    assert num > 0.0, 'Data should only contain positive values'
    total += num
print('total is:', total)



    ---------------------------------------------------------------------------

    AssertionError                            Traceback (most recent call last)

    <ipython-input-1-13c7d5640ddd> in <module>
          2 total = 0.0
          3 for num in numbers:
    ----> 4     assert num > 0.0, 'Data should only contain positive values'
          5     total += num
          6 print('total is:', total)


    AssertionError: Data should only contain positive values

def normalize_rectangle(rect):
    """ Normalizes a rectangle so that it is at the origin and 1.0 units long on its longest axis. input should be of the format (x0, y0, x1, y1).
    (x0, y0) and (x1, y1) define the lower left and upper right corners of the rectangle respectively."""
    assert len(rect) == 4, 'Rectangles must contain 4 coordinates'
    x0, y0, x1, y1 = rect
    assert x0 < x1, 'Invalid X coordinates'
    assert y0 < y1, 'Invalid Y coordinates'
    
    dx = x1 - x0
    dy = y1 - y0
    if dx > dy:
        scaled =dx / dy
        upper_x, upper_y = 1.0, scaled
    else:
        scaled = dx/ dy
        upper_x, upper_y = scaled, 1.0
        
    assert 0 < upper_x <= 1.0, 'Calculated upper x coordinate invalid'
    assert 0 < upper_y <= 1.0, 'Calculated upper y coordinate invalid'
    
    return (0, 0, upper_x, upper_y)
        

print(normalize_rectangle( (0.0, 1.0, 2.0)))
```


    ---------------------------------------------------------------------------

    AssertionError                            Traceback (most recent call last)

    <ipython-input-5-cb5ff8ce860f> in <module>
    ----> 1 print(normalize_rectangle( (0.0, 1.0, 2.0)))
    

    <ipython-input-4-54d27de53dd9> in normalize_rectangle(rect)
          2     """ Normalizes a rectangle so that it is at the origin and 1.0 units long on its longest axis. input should be of the format (x0, y0, x1, y1).
          3     (x0, y0) and (x1, y1) define the lower left and upper right corners of the rectangle respectively."""
    ----> 4     assert len(rect) == 4, 'Rectangles must contain 4 coordinates'
          5     x0, y0, x1, y1 = rect
          6     assert x0 < x1, 'Invalid X coordinates'


    AssertionError: Rectangles must contain 4 coordinates

print(normalize_rectangle( (4.0, 2.0, 1.0, 5.0)))
```


    ---------------------------------------------------------------------------

    AssertionError                            Traceback (most recent call last)

    <ipython-input-6-35750ccfc663> in <module>
    ----> 1 print(normalize_rectangle( (4.0, 2.0, 1.0, 5.0)))
    

    <ipython-input-4-54d27de53dd9> in normalize_rectangle(rect)
          4     assert len(rect) == 4, 'Rectangles must contain 4 coordinates'
          5     x0, y0, x1, y1 = rect
    ----> 6     assert x0 < x1, 'Invalid X coordinates'
          7     assert y0 < y1, 'Invalid Y coordinates'
          8 


    AssertionError: Invalid X coordinates

print(normalize_rectangle( (0.0, 0.0, 1.0, 5.0 )))
```

    (0, 0, 0.2, 1.0)


print(normalize_rectangle( (0.0, 0.0, 5.0, 1.0)))
```


    ---------------------------------------------------------------------------

    AssertionError                            Traceback (most recent call last)

    <ipython-input-8-83721d2716e7> in <module>
    ----> 1 print(normalize_rectangle( (0.0, 0.0, 5.0, 1.0)))
    

    <ipython-input-4-54d27de53dd9> in normalize_rectangle(rect)
         17 
         18     assert 0 < upper_x <= 1.0, 'Calculated upper x coordinate invalid'
    ---> 19     assert 0 < upper_y <= 1.0, 'Calculated upper y coordinate invalid'
         20 
         21     return (0, 0, upper_x, upper_y)


    AssertionError: Calculated upper y coordinate invalid




   
   
   
    ***_TRANSCRIPTION_***


    # Prompt the user to enter the input fasta file name

input_file_name = input('Enter the name of the input fasta file:')

    Enter the name of the input fasta file: fly gene.txt


# Open the input fasta file and read the DNA sequence

with open(input_file_name, "r") as input_file:
    dna_sequence = ""
    for line in input_file:
        if line.startswith(">"):
            continue
        dna_sequence += line.strip()

# Transcribe the DNA to RNA
rna_sequence = ""
for nucleotide in dna_sequence:
    if Nucleotide == "T":
        rna_sequence += "U"
    else:
        rna_sequence += nucleotide

# Prompt the user to enter the output file name

output_file_name = input("Enter the name of the output file: ")

    Enter the name of the output file:  fly gene.txt


# Save the RNA sequence to a text file

with open(output_file_name, "w") as output_file:
    output_file.write(rna_sequence)
print("The RNA sequence has been saved to {output_file_name}")

    The RNA sequence has been saved to {output_file_name}

print(rna_sequence)





