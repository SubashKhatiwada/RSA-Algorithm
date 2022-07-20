# RSA-Algorithm
#Key Generation
  1)	Use Miller-Rabin algorithm to choose two large primes, p and q.
  2)	Calculate n = pq
  3)	Calculate Φ(n) = (p – 1)(q – 1)
  4)	Select integer e
      GCD(Φ(n), e) = 1; 1 < e < Φ(n)
  5)	Calculate d = e^-1 mod Φ(n)
      //multiplicative inverse of  e under modulo Φ(n)
  6)	Public key PU = {e, n}
  7)	Private key PR = {d, n}
#Encryption
  1)	Plaintext: M < n
  2)	Ciphertext: C= M^e mod n
#Decryption
  1)	Ciphertext: C
  2)	Plaintext:  M= C^d mod n
