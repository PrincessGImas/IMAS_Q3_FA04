# Names of people
names = ["Me", "Lia", "Jake"]

# Steps per day for each person
steps = [
    [4500, 5200, 4800, 5000, 5300],
    [4000, 4100, 3900, 4200, 4600],
    [6000, 5800, 5900, 6100, 6200]
]

# Calculate total steps for each person
total_steps = []
for person_steps in steps:
    total = sum(person_steps)
    total_steps.append(total)

# Print total steps for each person
for i in range(len(names)):
    print(f"{names[i]} total steps: {total_steps[i]}")

# Identify person with the highest total
max_steps = max(total_steps)
max_index = total_steps.index(max_steps)
print(f"\nPerson with the highest steps: {names[max_index]} ({max_steps} steps)")

# Calculate and display difference between highest and lowest
min_steps = min(total_steps)
difference = max_steps - min_steps
print(f"Difference between highest and lowest total steps: {difference}")
