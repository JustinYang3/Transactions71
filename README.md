//main
Account acct1 = new Account("Ted Murphy", 72354);
	      Account acct2 = new Account("Jane Smith", 69713);
	      Account acct3 = new Account("Edward Demsey", 93757, 759.32);

	      acct1.deposit(25.85);

	      double smithBalance = acct2.deposit(500.00);
	      System.out.println("Smith balance after deposit: " +
	                          smithBalance);

	      System.out.println("Smith balance after withdrawal: " + 
	                          acct2.withdraw (430.75, 1.50));

	      acct1.addInterest();
	      acct2.addInterest();
	      acct3.addInterest();

	      System.out.println();
	      System.out.println(acct1);
	      System.out.println(acct2);
	      System.out.println(acct3);
        
// Account
public Account(String owner, long account, double initial)
   {
      name = owner;
      acctNumber = account;
      balance = 0;
   }
