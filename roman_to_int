integers = dict(I=1, V=5, X=10, L=50, C=100, D=500, M=1000)


class Solution:

    def romanToint(self, roman: str) -> int:
        result = 0
        for i, c in enumerate(roman):
            if i+1 < len(roman) and integers[roman[i]] < integers[roman[i+1]]:
                result -= integers[roman[i]]
            else:
                result += integers[roman[i]]
        return int(result)


roma = input()
arabic = Solution()
if 1 <= len(roma) <= 15:
    print(f"Input: {roma}")
    print(f"Output: {arabic.romanToint(roma)}")
else:
    print('Enter from 1 to 15 characters')
