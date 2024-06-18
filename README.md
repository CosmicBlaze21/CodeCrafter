import unittest
from codecrafter.challenge import Challenge
from codecrafter.solution import solve_challenge

class TestChallenges(unittest.TestCase):

    def test_sum_two_numbers(self):
        challenge = Challenge("Sum of two numbers", "sum_two_numbers")
        result = solve_challenge(challenge, [3, 5])
        self.assertEqual(result, 8)

if __name__ == '__main__':
    unittest.main()
