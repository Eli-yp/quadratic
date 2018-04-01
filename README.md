# quadratic
#给定a,b,c的值，计算出方程ax**2+bx+c=0的两个根

#-*- coding:utf-8 -*-                                                       
import math
import sys

def quadratic(a, b, c):
    data = b**2 - 4*a*c       #先给出判别式的表达
    #判别式的判断
    if data > 0:              #若data大于0             
        print('x1 = %s' % int((-b+data)/(2*a)))   #x1的表达式
        print("x2 = %s" % int((-b-data)/(2*a)))   #x2的表达式
    elif data == 0:           #若data等于0
        print('x1 = x2 = %s' % int((-b)/(2*a)))   #x1和x2相等
    else:
        print("方程无解")     #否则。若data小于0，方程无解
 a = int(sys.stdin.readline())
 b = int(sys.stdin.readline())
 c = int(sys.stdin.readline())
 quadratic(a,b,c)
                        
