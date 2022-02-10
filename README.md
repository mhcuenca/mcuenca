# mcuenca
l=len(players)
sum=0
for i in players:
    sum=sum+i
prom=sum/l
sum1=0
for i in players:
    sum1+=(i-prom)**2
desv=(sum1/(l-1))**0.5
cmin=prom-desv
cmax=prom+desv
cont=0
for i in players:
    if i>cmin and i<cmax:
        cont+=1
print(cont)
