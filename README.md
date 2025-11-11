words = {
    "apple": "a round fruit that grows on trees",
    "book": "a set of written or printed pages bound together",
    "computer": "an electronic device for storing and processing data",
    "teacher": "a person who helps others to learn",
    "student": "a person who studies at a school or university"
}

print("=== Welcome to Word Teacher ===")

score = 0
total = len(words)

# Main quiz loop
for word, meaning in words.items():
    print(f"\nWhat is the meaning of: {word}?")
    answer = input("Your answer: ")

    if answer.strip().lower() == meaning.lower():
        print("Correct ✅")
        score += 1
    else:
        print(f"Wrong ❌ The correct meaning is: {meaning}")

print("\n=== Quiz Finished! ===")
print(f"Your score: {score}/{total}")
print("Good job learning new words!")
