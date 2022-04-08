# lab-08.04
Задание 1
print(len(set(map(int, input().split()))))
Задание 2
print(len(set(input().split()) & set(input().split())))
Задание 3
print(*sorted(set(input().split()) & set(input().split()), key=int))
Задание 4
numbers = [int(s) for s in input().split()]
occur_before = set()
for num in numbers:
    if num in occur_before:
        print('yes')
    else:
        print('no')
        occur_before.add(num)
