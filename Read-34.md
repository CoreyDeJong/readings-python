## Django Best Practicies
- The Settings file is a small but very important part of any Django project. If you do it wrong, you’ll have a lot of issues during all phases of development. But if you do it right, it will be a good basis for your project that will allow it to grow and scale in the future.
- Keep settings in environment variables.
- Write default values for production configuration (excluding secret keys and tokens).
- Don’t hardcode sensitive settings, and don’t put them in VCS.
- Split settings into groups: Django, third-party, project.
- Follow naming conventions for custom (project) settings.

## SSH (Secure Shell)
- SSH, or Secure Shell, is a remote administration protocol that allows users to control and modify their remote servers over the Internet.
- The service was created as a secure replacement for the unencrypted Telnet and uses cryptographic techniques to ensure that all communication to and from the remote server happens in an encrypted manner. It provides a mechanism for authenticating a remote user, transferring inputs from the client to the host, and relaying the output back to the client.
- The significant advantage offered by SSH over its predecessors is the use of encryption to ensure secure transfer of information between the host and the client. - Host refers to the remote server you are trying to access, while the client is the computer you are using to access the host.
- Symmetric encryption is a form of encryption where a secret key is used for both encryption and decryption of a message by both the client and the host. 
- Symmetrical encryption is often called shared key or shared secret encryption. 
- Unlike symmetrical encryption, asymmetrical encryption uses two separate keys for encryption and decryption. These two keys are known as the public key and the private key. Together, both these keys form a public-private key pair.
- One-way hashing is another form of cryptography used in Secure Shell Connections. One-way-hash functions differ from the above two forms of encryption in the sense that they are never meant to be decrypted. They generate a unique value of a fixed length for each input that shows no clear trend which can exploited. This makes them practically impossible to reverse.