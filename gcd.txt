#Greatest common divisor calculator - by division algorithm


def divide(dividend, divisor):
  remainder = dividend % divisor
  #If remainder is 0, divisor is the gcd. Else divide divisor by remainder.
  if remainder == 0:
    return divisor
  else:
    return divide(divisor, remainder)
    

a = input("Enter dividend: ")
b = input("Enter divisor: ")
print "Greatest common denominator: " + str(divide(a, b))