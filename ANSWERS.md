<!-- Answers to the Short Answer Essay Questions go here -->

1. What is the purpose of using _sessions_?
<br>
sessions allow us to create state, using HTTP which on it's own is a stateless protocol. Using a unique session ID, tied to a unique user's cookie info, data can be persisted between page requests.
<br>
2. What does bcrypt do to help us store passwords in a secure manner.
<br>
bcrypt is a library developers can use, to hash and salt passwords before they are added to their database. The result is that the actual password isn't stored, rather the result of an algorithm applied to the original password. The hash aspect of the process transforms the original password, and the salt aspect of the process adds a unique value to the end of the password. 
<br>

3. What does bcrypt do to slow down attackers?
<br>
bcrypt uses a slow hashing algorithm, which in turns slows down attackers making the opportunity less attractive to an attacker. The slowing is accomplished by how many iterations of hashing are applied to the password. 
<br>
4. What are the three parts of the JSON Web Token?
<br>
The JSON Web Token is comprised of three main parts; header, payload, and signature. The header contains token type. The payload holds what is known as claims. Claims are information about the user (or other entity), and have three catagories; registered, public and private. Registered claims are recommended pieces of information, public claims are can be defined by anyone (precautions are recommended to avoid collisions), and private claims are customized to share information between parties in an agreed upon format. Finally, the third part of a JSON Web Token, the signature ensures a message wasn't changed in transit. 
<br>