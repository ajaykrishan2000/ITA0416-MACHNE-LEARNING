def find_s_algorithm(training_data):
    most_specific_hypothesis = training_data[0][:-1]
    for example in training_data:
        if example[-1] == "Yes":
            for i in range(len(most_specific_hypothesis)):
                if most_specific_hypothesis[i] != example[i]:
                    most_specific_hypothesis[i] = "?"
    
    return most_specific_hypothesis

training_data = [
    ["Sunny", "Warm", "Normal", "Strong", "Warm", "Same", "Yes"],
    ["Sunny", "Warm", "High", "Strong", "Warm", "Same", "Yes"],
    ["Rainy", "Cold", "High", "Strong", "Warm", "Change", "No"],
    ["Sunny", "Warm", "High", "Strong", "Cool", "Change", "Yes"]
]

most_specific_hypothesis = find_s_algorithm(training_data)
print("Most Specific Hypothesis:", most_specific_hypothesis)
