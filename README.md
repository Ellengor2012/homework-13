a = int(input("Сколько билетов вам нужно?"))
k = 1
sum_bel = 0
while k <= a:
    b = int(input(f"Билет номер {k}, Сколько лет человеку, который/которому покупает/покупается билет?"))
    if b < 18:
        k += 1
        continue
    elif 18 <= b < 25:
        k += 1
        sum_bel += 990
    elif b >= 25:
        k += 1
        sum_bel += 1390

if a > 3:
    sum_bel = sum_bel * 0.9

print(sum_bel)
