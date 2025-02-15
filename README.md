# culverkey

Culvkey is a chat app which has no sign up, login or usernames.  Both parties end up in the same channel if they have the same 
cryptographic key.  For now, only 1-on-1 chats are supported. 

Each party must decide how to call the chatroom. For instance, if Alice and Bob are chatting, it's responsibility of Alice to call the chatroom "Bob and me," while it's responsiblity of Bob to call the chatroom "Alice and me."  That's because there are no usernames or names. All chatters are anonymous.

The common cryptographic key is used for authentication, while the actual encryption uses the Signal protocol. 

The key must be communicated out of band. Optionally, the Crosspass app is integrated to assist with key transfer.

## UX Designs

Curverkey is as open source app. So far, the UX designs were completed. Developers are welcome to contribute implementation.
See mockups


## How it should be implemented

The exchanged encryption key is used as an HMAC key to sign elements of the protocol. The protocol itself must be the Signal protocol.

For mobile apps, use the Signal protocol library with a cross-platform toolkit like React Native or Flutter. Implement the server-side using Node.js. The Signal protocol is open-source and available for many platforms.
