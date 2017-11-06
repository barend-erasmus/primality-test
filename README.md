# Primality Test

A primality test is an algorithm for determining whether an input number is prime. Among other fields of mathematics, it is used for cryptography. 


## Fermat primality test

Formula:  `a^(n-1) % n = 1`

```javascript
const a = 2;
const n = 103;

const r = Math.pow(2, n - 1) % n;

if (r === 1) {
    console.log(`${n} is a prime number.`);
} else {
    console.log(`${n} is not a prime number.`);
}
```