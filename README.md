# FermatPrimalityTesting
Fermat's primality testing
Fermat's little theorem states that if p is prime and a is not divisible by p, then

    a^(p − 1) ≡ 1 ( mod p )

If one wants to test whether p is prime, then we can pick random integers a not divisible by p and see whether the equality holds. If the equality does not hold for a value of a, then p is composite. This congruence is unlikely to hold for a random a if p is composite. Therefore, if the equality does hold for one or more values of a, then we say that p is probably prime.

However, note that for a ≡ 1 ( mod p ), the above congruence holds trivially. It also holds trivially if p is odd and a ≡ − 1 ( mod p ). For this reason, one usually chooses a number a in the interval 1 < a < p − 1.

Any a such that

    a^(n − 1) ≡ 1 ( mod n )

when n is composite a is known as a Fermat liar. In this case n is called Fermat pseudoprime to base a.

If we do pick an a such that

    a^(n − 1) ≢ 1 ( mod n )

then a is known as a Fermat witness for the compositeness of n. 

------------ Example -------------
Suppose we wish to determine whether n = 221 is prime. Randomly pick 1 < a < 221, say a = 38. We check the above equality and find that it holds:

    a^(n − 1) = 38 220 ≡ 1 ( mod 221 ) .

Either 221 is prime, or 38 is a Fermat liar, so we take another a, say 24:

    a^(n − 1) = 24 220 ≡ 81 ≢ 1 ( mod 221 ) .

So 221 is composite and 38 was indeed a Fermat liar. Furthermore, 24 is a Fermat witness for the compositeness of 221. 
