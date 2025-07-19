These are the sevearal Sorting Techniques 
slectionsort
1.start from the fist element in the list/array
2.arr[0]=min
3.compare with all the remainingelement to find the reallowest element
4.perfom swapping with current position 
5.repeat same with adding positional values for each ,min check
 
 pseudo code
 for ->0to n-1:
 min=i
 for j->i+1 to n:
 if arr[j]<arr[(min)]
 swap
 min=i+1
        bubble sort
1.start from the begginng of the array
2.compare  each pair to adjacent number
3.if latest element is grater than adjacent prform swap
4.repeat the process till n-1
5.after each cycle/pass largest unsorted element would be in correct position
6.repeat passes till all the elemets are sorted
pseudo code:
for i ->0 to n-1:
for j->0 to n-i-2
if a[j]>a[j+1]
swap(a[j,a[j+]])
        csort
1.find max min of array
2.min!<0
3.create a count array to store frequency of numbers
4.modify the count array for each element to be store the sum of previous counts
5.place the output array back to the original array
pseudo code:
 countsort(arr,n):
 1.find max in arr
 2.create count (0-max)
 3.for i->0 to n-1:
 count[a[i]]+=1
 4.for i->1 to max_val:
 count[i]+=count[i-1]
 create output arr[n]
 5.for i->n-1 to 0:
 output [count[a[i]]-1]=a[i]
 count[a[i]]-=1
 copy output to arr
         Non counting sort
1.no -ve numbers
2.no -long numbers
3.short confined numbers only ex:0-100
                RADIX sort
ALGO:
1.find the maximum number to detrmine number of digits
2.select 10^0,for didgit position
3.increment digit position,w.r.t pass
4.loop->max_num//exp>0
perfom count sort based on current digit 
(num//exp)%10
multiply exp by 10
                Pancake Sort
Algo:
1.start with complete array and decrease the size(n-1)
2.for each size :
a.find a index of max element
b.flip the array with max size or max element imdex
c.flip the total array to current size
max->move to the end of the array 
3.repeat step1 by n-2,n-3......
for nth reduce element perfom step 2 untill 0 th index value respectivelly....
       
