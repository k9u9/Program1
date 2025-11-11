# Program1
Program# File Handling Example in Python

# Step 1: Create and write to the file
with open("sample.txt", "w") as file:
    file.write("Python is fun.\n")
    file.write("File handling is easy to learn.\n")
    file.write("We are writing and reading files in Python.\n")

print("Data written to sample.txt successfully!")

# Step 2: Read and display the file content
with open("sample.txt", "r") as file:
    content = file.read()
    print("\n--- File Content ---")
    print(content)

# Step 3: Count lines and words
with open("sample.txt", "r") as file:
    lines = file.readlines()
    line_count = len(lines)
    word_count = sum(len(line.split()) for line in lines)

print(f"\nTotal Lines: {line_count}")
print(f"Total Words: {word_count}")
