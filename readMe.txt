This Repository contains 2 packages(1 IS package + 1 Wm Test Suite package) , 1 ISSCCR report screen shot , 1 WmTest suite report screen shot

1) Install the Is package to the IS and try to execute the services thorough designer.
2) After installing , you can execute the services though below URLs too.Replace the host name and port as applicable.

	
HCF:

	1) To test multiple values:
		http://localhost:5555/invoke/CodeKata.exercise1.hcf.services/findHCD?inputs=98&inputs=56&inputs=112
	2) To test single value
		http://localhost:5555/invoke/CodeKata.exercise1.hcf.services/findHCD?inputs=98&inputs=0     
			/*added 0 value intentionally to handle string list */

JSON manipulations: (change the file name to local file path where addresses.json is present)

	1) To get pretty print of all addresses
	
		http://localhost:5555/invoke/CodeKata.exercise2.jsonManipulations.services/prettyPrint?filename=C:\Users\SHS\Desktop\addresses.json  

		
	2) To get formatted addresses.
		
		http://localhost:5555/invoke/CodeKata.exercise2.jsonManipulations.services/formatAddress?filename=C:\Users\SHS\Desktop\addresses.json
	
	3) To filter address based on type
	
	   
	   http://localhost:5555/invoke/CodeKata.exercise2.jsonManipulations.services/addressTypeFiltering?filename=C:\Users\SHS\Desktop\addresses.json&addressTypes=Physical Address&addressTypes=Postal Address
	   
	   http://localhost:5555/invoke/CodeKata.exercise2.jsonManipulations.services/addressTypeFiltering?filename=C:\Users\SHS\Desktop\addresses.json&addressTypes=Physical Address&addressTypes=                           
			/*added empty key at the end intentionally to handle string list */
			
	   http://localhost:5555/invoke/CodeKata.exercise2.jsonManipulations.services/addressTypeFiltering?filename=C:\Users\SHS\Desktop\addresses.json&addressTypes=Invalid Address&addressTypes=	
			
	 4) http://localhost:5555/invoke/CodeKata.exercise2.jsonManipulations.services/validateAddress?filename=C:\Users\SHS\Desktop\addresses.json
	 
String Calculator:

	  1) http://localhost:5555/invoke/CodeKata.exercise3.stringKata/stringCalculator?input=0
	  2) http://localhost:5555/invoke/CodeKata.exercise3.stringKata/stringCalculator?input=1
	  3) http://localhost:5555/invoke/CodeKata.exercise3.stringKata/stringCalculator?input=3,5,6,3,23
	  4) http://localhost:5555/invoke/CodeKata.exercise3.stringKata/stringCalculator?input=1\n2,3
	  5) http://localhost:5555/invoke/CodeKata.exercise3.stringKata/stringCalculator?input=//;\n1;2
	  6) http://localhost:5555/invoke/CodeKata.exercise3.stringKata/stringCalculator?input=1\n2,3
	  7) http://localhost:5555/invoke/CodeKata.exercise3.stringKata/stringCalculator?input=1\n-2,-3
	  8) http://localhost:5555/invoke/CodeKata.exercise3.stringKata/stringCalculator?input=2,1002
	  9) http://localhost:5555/invoke/CodeKata.exercise3.stringKata/stringCalculator?input=//[***]\n1***2***3
	  10)http://localhost:5555/invoke/CodeKata.exercise3.stringKata/stringCalculator?input=//[*][%]\n1*2%3        /* Url encoding required , replace % with %25
	  11)http://localhost:5555/invoke/CodeKata.exercise3.stringKata/stringCalculator?input=//[*][%][&]\n1*2%3&8   /* Url encoding required , replace % with %25 and replace & with %26

	  
	  
3) Install the WmTestSuite package and execute the test steps(Test Suite is created only for String Kata)
	  
	 
	 

		
		
	
	
	

