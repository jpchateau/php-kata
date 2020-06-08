php-kata
========

PHP skeleton for doing coding katas
-----------------------------------

*Code Kata* is a term coined by Dave Thomas, co-author of the book
The Pragmatic Programmer, in a bow to the Japanese concept of kata
in the martial arts. A code kata is an exercise in programming which
helps a programmer hone their skills through practice and repetition.

You can find some to start practicing [here](http://codingdojo.org/cgi-bin/index.pl?KataCatalogue).

When you do programming katas, you use TDD. That's why PHPUnit and Prophecy are included.

Practicing a kata
=================

Let's imagine you want to practice "Bowling game kata". Details about
this kata can be found [here](http://codingdojo.org/cgi-bin/wiki.pl?KataBowling).

You will need PHP >= 7.2 and [composer](https://getcomposer.org/).

```bash
$ composer install
```

You can also use a container ([Docker](https://www.docker.com/) is required):

```bash
$ docker build -t kata-php .
$ docker run -it --rm -v ~/path/to/data/:/usr/src/kata -name kata-php kata-php bash
```

Then, add your classes to `src/Kata` and your test cases to `src/Kata/Tests` and run your tests.

```bash
$ bin/phpunit
```

TestCase examples
=================

You will find one class and its TestCase in the project
in order to help you. You can delete them.

Adder is a class that adds two numbers and AdderTest tests that.

Run all the tests with this command:

```bash
$ bin/phpunit
```
