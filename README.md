# Hola JS Africa Challenge: string serching

Welcome to Hola's new JS programming challenge! Do you have the skills to write the fastest code? There's prize money at stake:

* First prize: 1500 USD.
* Second prize: 1000 USD.
* Third prize: 500 USD.
* We might also decide to award a 350 USD special prize for an exceptionally creative approach.

If you e-mail the link to this page to someone, with africa@hola.org in CC, and that someone enters the competition and wins a prize, you will receive the same amount, too!
For Hola, it's a chance to get to know many talented programmers, and to invite those who submit good code for job interviews.

Rules
This time, we tried to eliminate every possible way for subjective judgment to affect the outcome.
The fastest code, as long as it passes our correctness tests, wins.

* This challenge is open for anyone living in Africa.
  If you live elsewhere you are still
  welcome to submit your solution for fun - it will be evaluated and scored,
  but will not be eligable for a cash prize.
* Send your solution to africa@hola.org.
* Submission deadline: March 10, 2016, 23:59:59 UTC.
** Winner evaluation test-suite will be publicized on March 14, 2016.
  This will include a sample non-final performance results.
** Public discussion on test-suite, and adjustments according to valid feedback until March 21, 2016.
** Final performance results and winners will be publicized on March 28, 2016.
* You may submit more than once. Only your latest submission, as long as it's still before the deadline, will be evaluated.
* We will use Node.js v5.x.x (stable release at the time of this publication) for testing.
* Your code must all be in a single JS file.
* Your submission must be in pure JS. If you prefer CoffeeScript or similar, translate to JS before submitting -
  and attach your source in the original language (in addition to, not instead of JS).
* It is not allowed to require any JS modules, not even the standard ones built into Node.js.
* We will test your solution for both correctness and performance. Only solutions that pass the correctness
  testing will be admitted to performance testing. The fastest of the correct solutions wins.
* All submissions, as well as our correctness and performance tests, will be published after the end
  of the competition.
* Your full name (or a pseudonym if you sign your solution with one), but not your e-mail address,
  will be published.
* Do not publish your solution before the submission deadline, or you will be disqualified.
* If the problem statement seems ambiguous, check our reference implementation instead of asking
  us questions; but please do tell us if you suspect that the reference implementation
  contradicts this problem statement for a certain input.

# Problem Statement
You are in charge of developing a search engine. Your task is to write a Node.js module exporting one single function:
str_search(substrings, text)

Which will count occurences of substrings (up to 100 chars long) in large multi-megabyte text files,
and will return an Object with the number of occurrences of each of the substrings in text, case-sensitive.
All strings in the input are non-empty and only contain ASCII characters between 0x20 and 0x7F (inclusive).

Example:
str_search(['gsm', 'phone'], '') -> {gsm: 0, phone: 0}
str_search(['gsm', 'phone'], 'gsm-phones: Using a GSM phone in USA may be problematic') -> {gsm: 1, phone: 2}

# Reference implementation