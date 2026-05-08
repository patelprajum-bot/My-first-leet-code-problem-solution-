# My-first-leet-code-problem-solution-
Today I solved my first problem of lead code in 11 days of coding. It took me an over a year to solve it and after making a lot of mistakes I finally got it right.
MY ANSWER 
class Solution:
    def longestCommonPrefix(self, strs: List[str]) -> str:

        if not strs:
            return ""

        p = []

        strs.sort()

        for j in range(len(strs[0])):

            k = strs[0][j]

            if j < len(strs[-1]) and k == strs[-1][j]:
                p.append(k)
            else:
                break

        return "".join(p)
