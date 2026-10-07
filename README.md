# Kirchhoff-s-Laws
# Kirchhoff's Laws Calculator
# KCL and KVL

print("KIRCHHOFF'S LAWS CALCULATOR")
print("----------------------------")

print("\n1. Kirchhoff's Current Law (KCL)")
print("KCL: Sum of currents entering = Sum of currents leaving")

entering = float(input("Enter current entering the junction (A): "))
leaving1 = float(input("Enter first current leaving the junction (A): "))
leaving2 = entering - leaving1

print("Second current leaving the junction =",
      round(leaving2, 2), "A")

print("\n2. Kirchhoff's Voltage Law (KVL)")
print("KVL: Sum of voltage rises = Sum of voltage drops")

voltage_source = float(input("Enter source voltage (V): "))
voltage_drop1 = float(input("Enter first voltage drop (V): "))
voltage_drop2 = voltage_source - voltage_drop1

print("Second voltage drop =",
      round(voltage_drop2, 2), "V")

print("\nVerification:")
print("KCL:")
print("Entering current =", entering, "A")
print("Total leaving current =", round(leaving1 + leaving2, 2), "A")

print("\nKVL:")
print("Source voltage =", voltage_source, "V")
print("Total voltage drops =", round(voltage_drop1 + voltage_drop2, 2), "V")

print("\