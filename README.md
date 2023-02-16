m = int(input("Enter the number of rows: "))

n = int(input("Enter the number of columns: "))

#input of 1st Matrix

print("\nEnter Elements For 1st Matrix")

matrix1 = []

for i in range(m):

    row = []

    for j in range(n):

        element = int(input(f"Enter element at index ({i}, {j}): "))

        row.append(element)

    matrix1.append(row)

#input of 2nd Matrix

print("\nEnter Elements For 2nd Matrix")

matrix2 = []

for i in range(m):

    row = []

    for j in range(n):

        element = int(input(f"Enter element at index ({i}, {j}): "))

        row.append(element)

    matrix2.append(row)

#Print Matrix1

print("\nMatrix 1")

for row in matrix1:

        print(row)

#Print Matrix2

print("\nMatrix 2")

for row in matrix2:

        print(row)

#calculate the sum of the matrix

sum_matrix = []

for i in range(m):

    row = []

    for j in range(n):

        row.append(matrix1[i][j] + matrix2[i][j])

    sum_matrix.append(row)

#Print Sum Matrix

print("\nSum of Both Matrix")

for row in sum_matrix:

        print(row)

#calculate the difference of the matrix

diff_matrix = []

for i in range(m):

    row = []

    for j in range(n):

        row.append(matrix1[i][j] - matrix2[i][j])

    diff_matrix.append(row)

#Print Diff Matrix

print("\nDiff of Both Matrix")

for row in diff_matrix:

        print(row)

#calculate the product of the matrices

prod_matrix = []

for i in range(m):

    row = []

    for j in range(n):

        product = 0

        for k in range(n):

            product += matrix1[i][k] * matrix2[k][j]

        row.append(product)

    prod_matrix.append(row)

#Print Product Matrix

print("\nProduct of Both Matrix")

for row in prod_matrix:

        print(row)
