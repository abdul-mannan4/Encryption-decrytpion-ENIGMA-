1. Problem Statement
In today's digital world, communication within an organization plays a
vital role in maintaining smooth operations, improving productivity, and
ensuring coordination among team members. However, many organizations
face the challenge of securing sensitive internal communication from
unauthorized access. Simple messaging systems may not offer the necessary
protection against potential data breaches or unauthorized access.
This project aims to address these challenges by creating a secure
messaging system specifically for organizations, where communication is
restricted to within the organization. The system will allow users to send
messages to each other while ensuring that these messages are protected
through encryption. Additionally, it will allow administrators to manage user
accounts with essential functionalities such as creating new users, editing
passwords, and deleting accounts.
The primary objective of the system is to provide secure communication
where only the sender and the intended recipient can decrypt and read the
messages. To achieve this, a combination of two encryption techniques, Caesar
Cipher and Reverse Cipher, will be used. These ciphers, while basic in nature,
will ensure that messages cannot be easily understood by unauthorized
individuals, ensuring that privacy is maintained. The problem, therefore,
involves implementing a secure and efficient messaging system with user
management capabilities, providing both security and ease of use for all
members of the organization.
2. Solution
The solution to the problem is a C++-based application that provides
secure messaging between users within the same organization, with additional
administrative control for managing user accounts. The main components of
the solution include:
 Admin Management: Admins have full control over user accounts within
the organization. This means that they can view, create, edit, and delete
user accounts. However, admins do not have the ability to send or
receive messages within the system. Their role is purely administrative.
 User Messaging System: Users can log in to the system and send
encrypted messages to other users within the same organization. The
messages sent by users will be encrypted using a combination of Caesar
3
Cipher and Reverse Cipher to ensure that only the intended recipient
can decrypt and understand the message.
 Encryption & Decryption: The encryption system involves the use of two
classical ciphers:
o Caesar Cipher: This cipher shifts each letter of the message by a
certain number of positions in the alphabet. For example, if the
shift value (key) is 3, the letter "A" would become "D," "B" would
become "E," and so on. This provides basic encryption.
o Reverse Cipher: After applying the Caesar Cipher, the entire
message is reversed. This adds an additional layer of encryption
and further obfuscates the original message. Only the intended
recipient, who knows the decryption key, can reverse the process
and retrieve the original message.
 Secure Authentication: Only authenticated users of a specific chosen
organization can log into the system and access the messaging features.
Authentication will be done using usernames and passwords, ensuring
that only authorized individuals can access their accounts.
The system will utilize the Linked List data structure to store users and
admins information, allowing efficient management of dynamic data. 
