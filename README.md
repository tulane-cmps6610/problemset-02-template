# CMPS 6610: Problem Set 02

In this assignment, you will practice solving recurrences and implement the Karatsaba-Ofman algorithm. 

To complete this assignment, follow the instructions in [problemset-02.md](problemset-02.md) ([PDF version](problemset-02.pdf)). Below you'll find important and useful information about submitting your work, using git, and testing your code. 

## Turning in your work
- You may work with a partner to complete this assignment.
- Only one team member needs to push your completed lab to github. 
- At the top of `main.py` and in the `answers.md` file, **include the names of both** team members.
- Once you have pushed your final submission to GitHub, go to Canvas and submit a link to your repository to the Canvas assignment for this recitation. 
  - Submit to Canvas in group with your partner.

## Using Git 
- [Clone] your assignment repository to your local device.
- As you complete this lab, `add`, `commit`, and `push` your work up to GitHub. 
  - You will need to issue `git add` for all files that you have modified, e.g., `main.py`, `answers.md`, and any others that you modify or add to the repository as well.
  - For example, on the command line, in the same directory as your cloned lab:
    ```
    $ git add main.py
    $ git add answers.md
    $ git commit -m "Implement Required Functions, Answer all Questions"
    $ git push origin main
    ```
  - It is recommended that you `add`, `commit`, and `push` your work often in order to regularly save your work to GitHub. The latest version of your work will be what is graded.

## Running and testing your code
- You can run the tests using `pytest`. If you need to, install `pytest`. On your terminal:
  + `$ pip3 install pytest`
  + You may also have to install other python modules such as `tabulate` or other imported modules as you work through these recitations.
- It's usually best to run only one test at a time. To run tests, from the command-line, execute:
  + `$ pytest main.py` to run all tests
  + `$ pytest main.py::test_one` to just run `test_one`
  + If you are having trouble with your computer finding pytest after you've installed it, you can run it as follows:
    + `$ python -m pytest main.py`
  + GitHub will test your code using `pytest`.
- If your `python` is still defaulting to python version 2, explicitly use the `python3` executable instead. 

## About Markdown

We use Markdown extensively in these recitations. Markdown is a great way to easily add formatting to simple text documents.

Here is a [cheatsheet] for markdown syntax.

You will notice in the recitation documents that you can format mathematical expressions in markdown. To do so, wrap them in dollar signs. You can use [latex syntax] within the dollar signs. 

For example, the run time of our first example, linear search, this semester is $c_1n + c_2n + c_4 \in O(n)$. 

More generally, the runtime of any program can be expressed as:

$$\sum_i c_i * n_i$$

for every instruction $n_i$ and its cost $c_i$.

It's easy to do powers too. Euler's identity states: $e^{ix} + 1 = 0$

Pretty cool, huh?

You can also convert from markdown to pdf. `convert.sh` is provided for you to convert your `answers.md` to `answers.pdf`. As the comment in the script says, you will need to install pandoc and latex, but its pretty convenient to be able to do so. You do not need to submit you answers in PDF format, but you may if you like.

[Clone]: https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository-from-github/cloning-a-repository
[cheatsheet]: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
[latex syntax]: https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions


