Part III: better-ticket-machine project
48. the difference is that it will permit you to add the vlaue of zero to the balance

49. if(amount <= 0) {
            System.out.println("Use a positive amount rather than: " + amount);
        }else {
            balance = balance + amount;
        }
    
50. the boolean field was isVisible. yes it was well suited because it had only true or false

51. the code is in an if else statement, it adds price to the total instead of balance,
and it reduces your balance by the price instead of setting it to 0

52. It will compile but it won't do anything if the value insterted doesn't match
that of the condition

53. No, because the terminal will tell you that you need said amount of cents to 
print a ticket if you don't have enough.

55. public void multiply(){
        saving = price * discount;
    }
    
56. public void divide(){
        mean = total/count;
    }
    
57. if(price > budget){
            System.out.println("Too expensive");
        }else{
            System.out.println("Just right");
        }
        
58. if(price > budget){
            System.out.println("Too expensive. " + "Your budget is " + budget + " cents.");
        }else{
            System.out.println("Just right");
        }
        
59. it sets balance to 0 and returns 0

60. it returns the current balance before the refund then sets it to zero

61. sets price to 0

62. public void empty(){
        System.out.println(total);
        total = 0;
    }
    
63. public void printTicket()
    {
        amountLeftToPay = price - balance;
        if(amountLeftToPay <= 0) {
            
            // Simulate the printing of a ticket.
            System.out.println("##################");
            System.out.println("# The BlueJ Line");
            System.out.println("# Ticket");
            System.out.println("# " + price + " cents.");
            System.out.println("##################");
            System.out.println();

            // Update the total collected with the price.
            total = total + price;
            // Reduce the balance by the price.
            balance = balance - price;
        }
        else {
            System.out.printf("You must insert at least %d more cents.%n", amountLeftToPay);
        }