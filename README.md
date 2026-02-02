# compute-the-number-of-characters-words-and-lines-in-a-file.
f = open('D:/a.txt', 'r')

char, wc, lc = 0, 0, 0

for line in f:
    for i in range(0, len(line)):
        char += 1

        if line[i] == ' ':
            wc += 1

        if line[i] == '\n':
            wc += 1
            lc += 1

print("The no.of chars is %d\nThe no.of words is %d\nThe no.of lines is %d"
      % (char, wc, lc))

f.close()
