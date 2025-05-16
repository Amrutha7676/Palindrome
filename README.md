# Palindrome
def is_palindrome(s):
    # Remove non-alphanumeric characters and convert to lowercase
    cleaned = ''.join(char.lower() for char in s if char.isalnum())
    # Check if cleaned string is equal to its reverse
    return cleaned == cleaned[::-1]

# Example usage
user_input = input("Enter a word or phrase: ")
if is_palindrome(user_input):
    print("✅ It's a palindrome!")
else:
    print("❌ It's not a palindrome.")
