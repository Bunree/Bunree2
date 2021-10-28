a = open('1.txt', 'r')

b = a.read()
val = ['']

j = 0
summa = 0
for i in range(len(b)):
    if b[i] != ' ':
        val[j] += b[i]
    else:
        j += 1
        val.append('')

for i in range(len(val)):
    val[i] = int(val[i])

    print(val)
for f in range(len(val)):
    summa += val[f]
print(summa)

a.close()
