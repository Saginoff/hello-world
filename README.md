# hello-worldf
#
def arj(SN):
    usstor = []
    for i in range(SN[1]):
        usstor.append(int(input()))
    usstor.sort()
    k = 0
    for i in range(SN[1]):
        SN[0] -= usstor[i]
        if SN[0] < 0:
            return i


SN = list(map(int, input().split()))
print(arj(SN))
