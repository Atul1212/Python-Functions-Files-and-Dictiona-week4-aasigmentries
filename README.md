# Python-Functions-Files-and-Dictiona-week4-aasigmentries
1:-Write a function, sublist, that takes in a list of numbers as the parameter. In the function, use a while loop to return a sublist of the input list. The sublist should contain the same values of the original list up until it reaches the number 5 (it should not contain the number 5).



def sublist(L):

    b=[]
    n=0
    while L[n]!=5:

        b.append(L[n])

        n+=1
    return b

        


2:-Write a function called check_nums that takes a list as its parameter, and contains a while loop that only stops once the element of the list is the number 7. What is returned is a list of all of the numbers up until it reaches 7.




def check_nums(lst):

  sublist = []

  found = False

  while found == False:

    if lst[-0] != 7:

      sublist.append(lst[-0])

    else:
 found == True
      return sublist
      
      
      
      
      

    if len(lst) > 1:

      lst.pop(-0)

    else:

      break

  return sublist



3:-Write a function, sublist, that takes in a list of strings as the parameter. In the function, use a while loop to return a sublist of the input list. The sublist should contain the same values of the original list up until it reaches the string “STOP” (it should not contain the string “STOP”).



def sublist(string_list):

    sub = []

    try:
        stop_index = next(i for i in range(len(string_list)) if string_list[i] == "STOP")
        sub = string_list[:stop_index]

    except:
        sub = string_list
    return sub


4:-Write a function called stop_at_z that iterates through a list of strings. Using a while loop, append each string to a new list until the string that appears is “z”. The function should return the new list.



def stop_at_z(inputstr):

    d = 0 

    x=[]

    str1 = list(inputstr)

    while d<len(inputstr) :      

        if str1[d] == 'z' :
            break 
        else:           
            x.append(str1[d])
            d+=1
    return x 


4:-Below is a for loop that works. Underneath the for loop, rewrite the problem so that it does the same thing, but using a while loop instead of a for loop. Assign the accumulated total in the while loop code to the variable sum2. Once complete, sum2 should equal sum1.



sum1 = 0
lst = [65, 78, 21, 33]
for x in lst:
    sum1 = sum1 + x


