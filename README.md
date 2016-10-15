# Numerical-Stability
なぜ計算方法の違いによって値が変わるのか？
Ref:
Udacity -Deep Learning- Quiz:Numerical
Stabilityhttps://classroom.udacity.com/courses/ud730/lessons/6370362152/concepts/71235296110923#

その１
a = 1000000000
for i in range(100000):
    b = a + 0.000001
print(b-1000000000)
>>>9.5367431640625e-07

その２
a = 1000000000
for i in range(100000):
    a = a + 0.000001
print(a-1000000000)
>>>0.95367431640625
