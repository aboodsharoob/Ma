# Ma
def meme_calculator(a, b, op):
    if op == '+':
        result = a + b
    elif op == '-':
        result = a - b
    elif op == '*':
        result = a * b
    elif op == '/':
        result = a / b if b != 0 else "Infinity"
    else:
        return "Bruh, that's not an operation I know!"
    
    meme_responses = {
        42: "The answer to life, the universe, and everything 😎",
        69: "Nice.",
        420: "Blaze it!",
        1337: "Leet move bro!",
        "Infinity": "To infinity... and beyond!"
    }
    return meme_responses.get(result, f"Result: {result}")

# Example usage:
print(meme_calculator(21, 21, '+'))  # Will print "The answer to life, the universe, and everything 😎"
print(meme_calculator(70, -1, '+'))  # Will print "Nice."
