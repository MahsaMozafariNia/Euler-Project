#Multiples of 3 and 5

----------------------------------------------


	Sumation(n,a,b):

		S=0

		for i in range(1,n):

		if i%a==0 or i%b==0:

			S=S+i
          
		print (S)
   
	Sumation(n=1000,a=3,b=5)
___________________________________________________________________
___________________________________________________________________
#Even Fibonacci numbers

---------------------------------------------------
	def sumation(n):

	    list = [1, 2]

    	Sum = 2

		k = 0

    while k>=0:

        if (list[k]+list[k+1])%2 == 0 and list[k]+list[k+1] <= n:

            Sum = Sum+list[k]+list[k+1]

        if list[k]+list[k+1] <= n:

            list.append(list[k]+list[k+1])

            k = k+1

        else:

            k=-1

    print("sumation", Sum)

	sumation(4000000)
_____________________________________________________
_____________________________________________________

Largest Prime Factor

----------------------------------------------------------
	def LPF(n):

 	    for i in range (2,n):
	
      	  if n%i==0:
	
          	  return(LPF(n//i))

       	  if i==n-1:

         	  print(n)


	LPF(600851475143)
__________________________________________________
__________________________________________________

Largest palindrome product

-----------------------------------------------------
	m=[0]

	for j in range (999,99,-1):

	    for i in range(990,99,-1):

	        p=j*i

	        List=list(str(p))

	        if List==List[len(List)::-1]:

	            m.append(p)

	            i=99

	print(max(m))
