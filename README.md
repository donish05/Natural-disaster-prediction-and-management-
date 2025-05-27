# Natural-disaster-prediction-and-management-
Natural disaster prediction and management  description 

#def predict_tsunami(magnitude, depth, distance_to_coast):
    """
    Simple rule-based logic for tsunami prediction.
    """
    if magnitude >= 7.5 and depth <= 70 and distance_to_coast <= 300:
        return "Tsunami likely"
    elif magnitude >= 6.5 and depth <= 50 and distance_to_coast <= 100:
        return "Tsunami possible"
    else:
        return "No tsunami"

# Optional: Get input from user
try:
    magnitude = float(input("Enter earthquake magnitude (e.g. 7.8): "))
    depth = float(input("Enter depth in km (e.g. 40): "))
    distance_to_coast = float(input("Enter distance to coast in km (e.g. 150): "))

    result = predict_tsunami(magnitude, depth, distance_to_coast)
    print("Prediction:", result)

except ValueError:
    print("Please enter valid numbers.")

Output:
Enter earthquake magnitude (e.g. 7.8): 7.8
Enter depth in km (e.g. 40): 40
Enter distance to coast in km (e.g. 150): 150
Prediction: Tsunami likely
