# cathrin97
from random import randint
i0 = randint (1,10)
j0 = randint (1,10)
i1 = randint (1,10)
j1 = randint (1,10)
while (i0 != i1) or (j0 != j1):
    x = raw_input('Give me direction')
    if (x !='left') and (x != 'right') and (x !='down') and (x !='up'):
        print 'Try again'
    else:
        if x == 'left':
            if (j0-1) != 0:
                j0 = j0-1
                if j0 > j1:
                    print 'Απόσταση στηλών',j0-j1
                else:
                    print 'Απόσταση στηλών',j1-j0
            else:
                print raw_input('Choose another direction')
        elif x == 'right':
            if (j0+1) != 0:
                j0 = j0+1
                if j0 > j1:
                    print 'Απόσταση στηλών',j0-j1
                else:
                    print 'Απόσταση στηλών',j1-j0
            else:
               print raw_input('Choose another direction')  
        elif x == 'down':
            if (i0+1) != 0:
                i0 = i0+1
                if i0 > i1:
                    print 'Απόσταση γραμμών',i0-i1
                else:
                    print 'Απόσταση γραμμών',i1-i0
            else:

                print  raw_input('Choose another direction')
        else:
            if (i0-1) != 0:
                i0 = i0-1
                if i0 > i1:
                    print 'Απόσταση γραμμών',i0-i1
                else:
                    print 'Απόσταση γραμμών',i1-i0
            else:
                print raw_input('Choose another direction')        
            
print 'Congratulations!!!You found the treasure!!!'

