# Goldman-Sachs-Engineering-Virtual-program-
Goldman Sachs Virtual  program 


                         MEMORUNDUM 

DATE : September 29 2021         SUBJECT : Crack leaked password database

FROM : Ansong Evans                TO : Goldman Sachs	 

  QUESTIONS

  What type of hashing algorithm was used to protect passwords ?
  
- SHA512crypt  function that was included by default in Mac OS X and examples of other similarly "slow" hashing algorithms include bcrypt, scrypt, PBKDF2
What level of protection does the mechanism offer for passwords?
  
- it offers a secure way to store user’s passwords and prevent data from being compromised by  third parties who may gain access to the database. 
  
What controls could be implemented to make cracking much harder for the hacker in the event of a password database leaking again ?
  
- Use a dedicated password hashing algorithm bcrypt, scrypt or PBKDF2 as this will greatly increase the time needed to crack individual passwords.
- Implement SALTING  to prevent usage of rainbow tables to speed up cracking.
  
What can you tell about the organization’s password policy (e.g. password length, key space, etc.) ?
- Weak minimum password length and no specific requirements.
  
What would you change in the password policy to make breaking the passwords harder ?
  
- Avoid common words and character combinations in your password.
- Longer passwords are better, 8 characters length should be the minimum required password. 
- Don’t reuse your passwords on all web portals and Include special character, Capital and Small letters, numbers in your password
- Users should  Include special character, Capital and Small letters, numbers in your password.
- Don’t let users include their username, actual name, date of birth and other personal information while creating a password.

For example :
ilovetopror!amcomputers! (Pass) => Hash function + [ Salt will be generated and added on] => $2b$10$gya/iCuX628wh3u1uGzXiuSZPl6jBcch8z2BoXnqeXTjnAKN
