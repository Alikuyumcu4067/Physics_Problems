def calculate_momentum(mass_grams, velocity_ms):
    # Convert mass from grams to kilograms for SI units
    mass_kg = mass_grams / 1000
    # Momentum formula: p = m * v
    return mass_kg * velocity_ms

# Data for the objects
fly = {"name": "Fly", "mass": 2, "velocity": 10}
ball = {"name": "Tennis Ball", "mass": 60, "velocity": 1}

# Calculate momentum for both
p_fly = calculate_momentum(fly["mass"], fly["velocity"])
p_ball = calculate_momentum(ball["mass"], ball["velocity"])

# Output results
print("--- Momentum Comparison ---")
print(f"{fly['name']} Momentum: {p_fly:.3f} kg·m/s")
print(f"{ball['name']} Momentum: {p_ball:.3f} kg·m/s")
print("-" * 27)

if p_ball > p_fly:
    print(f"Result: The {ball['name']} has greater momentum.")
elif p_fly > p_ball:
    print(f"Result: The {fly['name']} has greater momentum.")
else:
    print("Result: Both have equal momentum.")
