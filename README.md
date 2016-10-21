# CS _Internship_ Questionnaire

## Purpose and General Instructions
This questionnaire is intended to help us pre-screen applicants to our software development internship position. Submissions should be made in the form of a [secret gist](https://gist.github.com) (for help creating gists, see this [article](https://help.github.com/articles/creating-gists/)). You will send the link to that gist to the email address _provided to you when you were sent the link to this challenge_. **NOTE: Unsolicited gists will be _completely ignored_. You must apply for the position and be asked to submit a gist before sending one.**

Your submission should be a single gist, but you may have multiple files within the submission if desired (e.g: one file per coding challenge, and one file with the answers to all the questions).

## Technical Questions
Please answer the following questions, in your own words, to the best of your ability, (as part of the gist) with a few full and complete sentences per response:

  1. In HTML, what are the differences between a `<div>` and a `<span>`?

  2. What is the difference between a `class` and `id` in HTML/CSS?

  3. What Linux/Unix command would you use to find all files with _contents_ including a particular string in a given folder?

  4. Why is Bubble Sort bad?

  5. Compare/Contrast XML with JSON. What strengths does each format offer?

  6. What regular expression would you use to _reasonably_ match an email address?

  7. Why are powers of 2 important in Computer Science?

  8. What is polymorphism?

  9. What are database transactions and when would you use one?

  10. ~~Does P = NP?~~

## Coding Micro-Challenges
Please submit solutions to the following challenges in the language(s) of your choice (_preferred_ languages include: C++, Java, JavaScript, Ruby, PHP, Python, Scala):

  1. Write a function that takes in a positive integer (hereby referred to as N) and returns the first N _odd integers_ as an array (or some other iterable object). Ex:
  ```
    odds(2) => [1, 3]
    odds(4) => [1, 3, 5, 7]
  ```

  2. Write a function that takes a positive integer (N) as an exponent, which returns the base-10 sum of the base-10 _digits_ of 2^N. Ex:
  ```
    2^3 = 8 => 8
    2^4 = 16 => 1 + 6 = 7
    2^10 = 1024 => 1 + 0 + 2 + 4 = 7
    2^11 = 2048 => 2 + 0 + 4 + 8 = 14
  ```

  3. Write a `Plant` class with a `name` (string) attribute, a `size` attribute (initially `1`), a `grow` method which increases the plant's size by `1`, and a `die` method which destroys/deletes that `Plant`.

  4. Write an `Animal` class with a `name` (string) attribute, a `size` attribute (initially `1`), an `eat` method which takes either a `Plant` instance or an `Animal` instance as the argument and returns nothing, and a `die` method which destroys/deletes that `Animal`.

  5. Write a `Carnivore` class which inherits from `Animal`. Its `eat` method should invoke `die` on the `Plant` or `Animal` eaten, and do the following:
    - If the object eaten was a `Plant`, the `Carnivore` should decrease its size by 1 (if it reaches `0`, it should `die`).
    - If the object eaten was an `Animal`, it should increase its `size` by the `size` of the animal eaten.
