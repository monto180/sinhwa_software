#백준 2558
a = int(input())
b = input()
print(a*int(b[2]))
print(a*int(b[1]))
print(a*int(b[0]))
print(a*int(b))

--------------------------------------------------

#백준 1212
print(bin(int(input(), 8))[2:])

--------------------------------------------------

#백준 1252
a, b = input().split()
sum = int(a,2) + int(b,2)
print(bin(sum)[2:])

--------------------------------------------------

#백준 1271
a, b = map(int, input().split())
print(a //b)
print(a%b)

--------------------------------------------------

#백준 1373
print(oct(int(input(), 2))[2:])

--------------------------------------------------

#백준 2455
on = []
people = 0
for _ in range(4):
    a, b = map(int, input().split())
    people += b
    people -= a
    on.append(people)
print(max(on))

--------------------------------------------------

#백준 2530
h, m, s = map(int, input().split())
t = int(input())
s += t%60
t = t //60
if s>= 60:
    s-= 60
    m+=1
m += t%60
t =t //60
if m>= 60:
    m-= 60
    h+=1
h += t%24
if h>= 24:
    h-= 24
print(h,m,s)

--------------------------------------------------

#백준 2903
a = int(input())
print((2**a + 1)**2)

--------------------------------------------------

#백준 1330
a, b = map(int, input().split())
if a > b:
    print(">")
elif a<b:
    print("<")
else:
    print("==")

--------------------------------------------------

#백준 9498
test_score = int(input())
if 100 >= test_score >= 90:
    print("A")
elif 89 >= test_score >= 80:
    print("B")
elif 79 >= test_score >= 70:
    print("C")
elif 69 >= test_score >= 60:
    print("D")
else:
    print("F")

--------------------------------------------------

#백준 2753
year = int(input())
if (year%4 == 0 and year%100 !=0) or (year %400 ==0):
    print(1)
else:
    print(0)

--------------------------------------------------

#백준 14681
x = int(input())
y = int(input())
if x > 0 and y>0:
    print(1)
elif x<0 and y>0:
    print(2)
elif x<0 and y<0:
    print(3)
else:
    print(4)

--------------------------------------------------

#백준 2490
yut = list(map(int, input().split()))
zeros = yut.count(0)
if zeros == 1: print("A")
elif zeros == 2: print("B")
elif zeros == 3: print("C")
elif zeros == 4: print("D")
else: print("E")
yut = list(map(int, input().split()))
zeros = yut.count(0)
if zeros == 1: print("A")
elif zeros == 2: print("B")
elif zeros == 3: print("C")
elif zeros == 4: print("D")
else: print("E")
yut = list(map(int, input().split()))
zeros = yut.count(0)
if zeros == 1: print("A")
elif zeros == 2: print("B")
elif zeros == 3: print("C")
elif zeros == 4: print("D")
else: print("E")

--------------------------------------------------

#백준 2839
n = int(input())
bag = 0
while n >= 0:
    if n%5==0:
        bag+=n//5
        print(bag)
        break
    n -=3
    bag+=1
else:
    print(-1)
