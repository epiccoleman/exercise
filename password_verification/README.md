# Password Verification

You are the head of security at the Depository Bank of Zurich and are responsible for your customers logging into your secure banking system to retrieve their private items from their secure safety deposit boxes. 

Some customers enter the bank, blabbing about the Holy Grail. You don’t know what they are talking about, but they sound very important so you rush to get them logged into their account only to find that the authentication system has been corrupted! 

Since your job is on the line, and you have some very important customers at your door, you decide to start diagnosing the problem by hand.

To troubleshoot, you have decided to come up with a list of passwords and their associated rules at the time of the password creation.

For example, suppose you have the following list:

```
1-3 a: abcde
1-3 b: cdefg
2-9 c: ccccccccc
```

Each line gives the password policy and then the password. The password policy indicates the lowest and highest number of times a given letter must appear for the password to be valid. For example, `1-3 a` means that the password must contain `a` at least `1` time and at most `3` times.

In the above example, `2` passwords are valid. The middle password, `cdefg`, is not; it contains no instances of `b`, but needs at least `1`. The first and third passwords are valid: they contain one `a` or nine `c`, both within the limits of their respective policies.

Given our input, how many passwords are valid according to their policies?

Original problem adapted from [Advent of Code 2020](https://adventofcode.com/2020/day/2) 
