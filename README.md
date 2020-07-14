# MiniBlocklyChain

![imagen](https://user-images.githubusercontent.com/60530547/86207891-1ea4d080-bb35-11ea-84d2-1b9aee22cf97.png)

By www.OpenQbit.com


The opensource version of Mini BlocklyChain, is a blockchain based on Blockly programming for App Inventor and others blockly systems. Information is available at languages ​​(Spanish, English, Chinese, German, French, Italian, Japanese, Dutch and Portuguese).

Mini BlocklyChain is a fully functional blockchain is a technology developed for mobile phones with OS (Operating System) Android that will be the nodes that will perform in sending and receiving transactions. We created the first blockchain technology that is structured in a "modular" way through Blockly programming where anyone with minimal knowledge and without knowing how to program can create and develop programs for mobile phones and create their own blockchain either in public or private network mode. If you want to create your own digital currency you can do it or a solution to use it in a company, the possibilities are based on the needs of each real case and the business logic that the user adopts or creates according to his requirements.

Mini BlocklyChain is the first modular blockchain for mobile phones where a transactional system can be implemented in a short time.

Before entering the definition and use of "module" blocks we need to have the basic concepts of the Mini BlocklyChain components to know when, how and where to apply them according to the real case we want to implement.
The following concepts emphasize what type of user they are targeting, so it is not important for people who do not have programming skills that the concepts for development users are fully understood. 

To review the way of use, there is a user manual created to implement a blockchain system from scratch.

The manuals are found in the "HandBooks" directory in the following languages ​​(Spanish, English, Chinese, German, French, Italian, Japanese, Dutch and Portuguese).

Extensions are found in the "Extensions" directory which are described in detail in the user manual.

The different extensions that provide us with levels of security to save, validate and transfer transactions from the Mini BlocklyChain network nodes.

The security blocks are based on the following extensions:

I.	  OpenQbitAESEncryption extension.

II.	  OpenQbitAESDecryption extension.

III.	OpenQbitAEStoString extension.

IV.	  OpenQbitEncDecData extension.

V.	  OpenQbitFileHash extension.

VI.	  OpenQbitRSA extension.

VII.	OpenQbitSSHClient extension.

VIII.	OpenQbitStringHash extension.

IX.	  OpenSQLite extension.

X.    OpenQbitBlock extension.

We have implemented a consensus algorithm based on quantum computing which we call PoQu (Proof of Quantum).

PoQu. - "Proof of Quantum" is a consensus algorithm developed for Mini BlocklyChain, this test is a variant of the Proof of Work (PoW) that works as follows.
The Proof of Quantum (PoQu) at startup is executed with the same algorithm as the "Proof of Work" (PoW) is based on putting the processor of the device (PC, Server, Tablet or Mobile Phone) to work to obtain a string of characters that is a mathematical puzzle called a "hash".

Remember that a "hash" is an algorithm or mathematical process that when introducing a phrase or some type of digital information such as text files, program, image, video, sound or other diverse type of digital information gives us as a result an alphanumeric character that represents the digital signature that represents it in a unique and non-repeatable way of the data, the hash algorithm is unidirectional, this means that when you enter a data to obtain its signature "hash" its reverse process can not be performed, having a signature "hash" we can not know what information was obtained this property gives us a security advantage to process the information we send over the Internet. How does it work? Imagine sending any kind of information through non-secure channels and accompany it with its respective "source hash", the receiver when receiving the information can get the "hash" of the information received we will call it "destination hash" and check it with the "source hash" if both "hashes" are the same we can confirm that the information has not been altered in the channel that was sent, is just an example where this type of information security process is currently used.

Currently there are different types of algorithms or hash processes that differ in the level of security. The most used or known are: MD5, SHA256 and SHA512.

Example of SHA256:

We have a chain or sentence as follows: "Mini BlocklyChain is modular. If we apply a SHA256 hash to the previous string it will give us the next hash.

f41af7e61c3b02fdd5e5c612302b62a2dd52fcb38f9of97cb2afd827e8804db8

The above alphanumeric string is the signature that represents the sentence in the above example

For more example we can use the site on the internet:
https://emn178.github.io/online-tools/sha256.html


In the case of the "Test Work" (PoW) algorithm, it works by using computing power to obtain a predefined hash.

Let's imagine that we have the previous "hash" that we took from the "Mini BlocklyChain is modular" chain.

f41af7e61c3b02fdd5e5c612302b62a2dd52fcb38f9of97cb2afd827e8804db8

To this "hash" in its beginning we put the parameter of difficulty that is simply to put zeros "0" in the beginning, that is to say if we say that the difficulty is of 4 it will have "0000" + "hash" to this we will call it "seed hash"

0000 f41af7e61c3b02fdd5e5c612302b62a2dd52fcb38f9de97cb2afd827e8804db8

Now taking into account that we know the input information that is the string: "Mini BlocklyChain is modular" we add at the end of the string a number starting from zero "0" and we take out its hash to this we will call it "hash nonce":

f41af7e61c3b02fdd5e5c612302b62a2dd52fcb38f9de97cb2afd827e8804db80

We got hash nonce:
7529f3ad273fc8a9eff12183f8d6f886821900750bb6b59c1504924dfd85a7c8

Then we perform a comparison of the new "hash nonce" with the "hash seed" if they are equal the node that first finds the equality will win the execution of processing the current transaction. As we can see this process is based on probability and computational strength of the device which gives the "Proof of Work" test a consensus equity for all nodes.

If the "seed hash" does not coincide with the "hash nonce", the difficulty is increased by one and the "hash nonce" is removed again, the number that is being increased is called the "nonce" number, it is compared with the "seed hash" until they coincide or are the same. 

As we can see the number "nonce" or increase is the one that will help to obtain the "hash" of equality.

Based on the "Proof of Work" (PoW) algorithm, the Proof of Quantum (PoQu) algorithm is based on obtaining the number "nonce" as PoW does and using a minimum level difficulty ranging from 1 to 5, this serves only to the mobile device to gain the right to be a candidate to win the consensus.

The Proof of Quantum (PoQu), is activated when the mobile phone has finished the minimum PoW and wins the pass to obtain a probability number in the QRNG system.

The QRNG (Quantum Random Number Generator) is a Quantum Random Number Generator, this system is based on generating true random numbers based on quantum mechanics is the safest system today to generate such numbers. For more details see Annex "Quantum Computation with OpenQbit".

Mini BlocklyChain can implement both minimum PoW and PoQu concession types.

The PoQu Proof is based on obtaining the number "nonce" this number in the PoQu Proof is known as "Magic Number" with this the "Peer to Peer" system will confirm if the number is correct and then a random number will be obtained with the QRNG server pool. This random number will be registered in all the nodes, a list will be created containing ((Node Sum /2)) +1 and from this list the one with the highest percentage of probability to be the winner candidate of the consensus (PoQu) will be chosen and this one will execute the current transaction queue.

The PoQu algorithm also uses NIST (National Institute of Standards and Technology) testing to assure us that the random numbers in the QRNG are truly random numbers.
https://nvlpubs.nist.gov/nistpubs/legacy/sp/nistspecialpublication800-22r1a.pdf

In Mini BlocklyChain we have implemented a block for PoW and a block for PoQu.

These blocks use a type of hash: SHA256 for free use, for commercial use you have a SHA512 and other types of hash as required.

For more details on the concept of HASH see:
https://es.wikipedia.org/wiki/Funcion_hash

NOTE: The Proof of Work (PoW) used in mobile phones can only use a maximum difficulty of 5 since the mathematical processing of these devices is not dedicated like servers or PCs. We only use the PoW algorithm to obtain the opportunity to obtain your pass or permission to enter the Quantum Random Number Generator (QRNG) system and with it to execute the Quantum Random Number Generator (PoQu) algorithm.

On mobile phones do not use a maximum difficulty of 5 as the system may lock up and not respond properly.

More information.
www.openqbit.com

Regards
Guillermo Vidal.


