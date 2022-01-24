
4. Top 3 Max Lucky Winners
import time

def findmax(sequence):
    max = sequence[0]
    index = 0
    for i in range(len(sequence)):
        if (sequence[i] > max):
            max = sequence[i]
            index = i
    return (max,index)

start = time.time()

input = [1,6,3,8,9,10,7,4]#[10,0,-5,20,7,9,11]

#Top1
print(input)
max1,index = findmax(input)
print(max1,index)
input.remove(max1)

#Top2
print(input)
max2,index = findmax(input)
print(max2,index)
input.remove(max2)

#Top3
print(input)
max3,index = findmax(input)
print(max3, index)
print(max1,max2,max3)

print("The time taken is ", time.time()-start, "seconds.")
