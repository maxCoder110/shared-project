# shared-project
import random

def generate_random_numbers(count, lower_bound, upper_bound):
    """Generate a list of random integers within a specified range.

    Args:
        count (int): The number of random integers to generate.
        lower_bound (int): The lower bound of the range (inclusive).
        upper_bound (int): The upper bound of the range (inclusive).

    Returns:
        list: A list containing the generated random integers.
    """
    return [random.randint(lower_bound, upper_bound) for _ in range(count)]
if __name__ == "__main__":
    num_count = 10
    lower = 1
    upper = 100
    random_numbers = generate_random_numbers(num_count, lower, upper)
    print(f"Generated {num_count} random numbers between {lower} and {upper}:")
    print(random_numbers)

