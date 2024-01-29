Problem 1
result = [] for number in range(2000, 3201): if number % 7 == 0 and number % 5 != 0: result.append(str(number))

print(",".join(result))

Problem 2
def square_dictionary(n): square_dict = {} for i in range(1, n+1): square_dict[i] = i * i return square_dict

n = int(input("Enter an integer n: ")) result_dict = square_dictionary(n)

print("The dictionary of squares is:") for key, value in result_dict.items(): print(f"{key}: {value}")

Problem 3
def factorial(n): if n == 0: return 1 else: return n * factorial(n - 1)

num = int(input("Enter a number: "))

if num < 0: print("Factorial is not defined for negative numbers.") else: factorials = [str(factorial(i)) for i in range(num + 1)] result = ",".join(factorials) print("Factorials of numbers from 0 to", num, "are:", result)

Problem 4
input_str = input("Enter a sequence of comma-separated numbers: ")

num_list = [int(num) for num in input_str.split(',')]

num_tuple = tuple(num_list)

print("List:", num_list) print("Tuple:", num_tuple)
