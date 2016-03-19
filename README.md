# python-zadania-19.03
część zadań z cw 3 i wielomian
###Napisz skrypt który wykonuje nastpujaca operacje 
1. Buduje liste kodujaca wielomian W(x)=2x^4+4x^3+x+7
2. Wyswietla wartosc wielomianu w punkcie x=3
3. Wyswietla wykres wielomianu z zaznaczonym punktem x=3

```python
import numpy as np
import matplotlib.pyplot as plt
import numpy.random as npr

W1=[2,4,0,1,7]
a=np.polyval(W1,3)
print(a)
x=np.linspace(-4,4,101)
y=np.polyval(W1,x)
plt.plot(x,y)
plt.plot(3,a,'o')

