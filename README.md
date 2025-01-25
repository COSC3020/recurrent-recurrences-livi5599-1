# Recurrent Recurrences

Give big $\Theta$ bounds for the following recurrence relations.

1.
$$ T(n) =
    \begin{cases}
        1 & n \leq 1\\
        T\left(\frac{n}{13}\right) + 5 & n > 1
    \end{cases}
$$

2.
$$ T(n) =
    \begin{cases}
        1 & n \leq 1\\
        13 T\left(\frac{n}{13}\right) + 5 & n > 1
    \end{cases}
$$

3.
$$ T(n) =
    \begin{cases}
        1 & n \leq 1\\
        13 T\left(\frac{n}{13}\right) + 2n & n > 1
    \end{cases}
$$

1. $\Theta(log(n))$.  This is because from the substitution method, I determined the general case of T(n/13) + 5 is T(n/13^i) + 5i.  I then replaced i with log13(n), which led me to the answer of $\Theta(log(n))$.

2. $\Theta(n)$.  This is because from the substitution method and the use of the finite geometric series formula, I determined the general case of 13T(n/13) + 5 is 13^i * T(n/13^i) + 5 * (13^(i + 1) - 1)/12.  I then replaced i with log13(n), which led me to the answer of $\Theta(n)$.

3. $\Theta(n * log(n))$.  This is because from the substitution method, I determined the general case of 13T(n/13) + 2n is 13^i * T(n/13^i) + 2n * i.  I then replaced i with log13(n), which led me to the answer of $\Theta(n * log(n))$.

-----

I used ChatGPT to give me the finite geometric series formula.  I then solved the equation using the formula on my own.

I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models.  All of the work is my own, except where stated otherwise.  I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.

-----

I submitted this assignment last semester.
