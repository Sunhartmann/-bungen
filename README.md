# Übungen
DNAString = 'TAAGATTCTAAGATTCCGGGCTCGCCCG'
pattern_len = 4
DNA_variable = {}

for i in range(len(DNAString)-pattern_len):
    text = DNAString[i:i+pattern_len]
    if text not in DNA_variable:
        DNA_variable[text] = 0
    else:
        DNA_variable[text] += 1
for k in DNA_variable:
    if DNA_variable[k] == max(DNA_variable.values()):
            print(k)
