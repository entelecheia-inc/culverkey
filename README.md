# culverkey

Culvkey is a chat app which has no sign up, login or usernames.  Both parties end up in the same channel if they have the same 
cryptographic key.  For now, only 1-on-1 chats are supported. 

Each party must decide how to call the chatroom. For instance, if Alice and Bob are chatting, it's responsibility of Alice to call the chatroom "Bob and me," while it's responsiblity of Bob to call the chatroom "Alice and me."  That's because there are no usernames or names. All chatters are anonymous.

The common cryptographic key is used for authentication, while the actual encryption uses the Signal protocol. 

The key must be communicated out of band. Optionally, the Crosspass app is integrated to assist with key transfer.
