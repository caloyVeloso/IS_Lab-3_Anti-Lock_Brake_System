# IS_Lab-3_Anti-Lock_Brake_System

# Fuzzy Logic Brake Control System

## Description

This project implements a fuzzy logic control system for brake actuation based on vehicle speed and brake pressure. Fuzzy logic is a mathematical approach to computing that accounts for uncertainty and imprecision, making it suitable for control systems where precise mathematical models are challenging to define.

## System Components

### Input Variables
1. **Vehicle Speed:** Membership functions for 'slow,' 'medium,' and 'fast' speeds.
2. **Brake Pressure:** Membership functions for 'none,' 'light,' 'moderate,' and 'heavy' pressure.

### Output Variable
- **Brake Actuation:** Membership functions for 'release,' 'partial_application,' and 'full_application.'

## Rules

The system includes a set of fuzzy rules that define the relationship between the input variables and the output variable. Rules consider different combinations of vehicle speed and brake pressure to determine the appropriate brake actuation.

## Usage

1. Create a fuzzy control system using the defined rules and membership functions.
2. Provide input values for vehicle speed and brake pressure.
3. Compute the result of the fuzzy logic system to obtain the brake actuation.

## Visualization

The system includes visualizations of the fuzzy membership functions and rules for vehicle speed, brake pressure, and brake actuation. These visualizations help in understanding the behavior of the fuzzy logic system.

## Example

```python
# Example Usage

# Create the control system
system = ctrl.ControlSystem([rule1, rule2, rule3, rule4, rule5, rule6, rule7, rule8, rule9, rule10, rule11, rule12])

# Create a simulation
brake_system = ctrl.ControlSystemSimulation(system)

# Provide input values
brake_system.input['vehicleSpeed'] = speed_input
brake_system.input['brakePressure'] = brake_pressure_input

# Compute the result
brake_system.compute()

# Access the output value
output_value = brake_system.output['brakeActuation']

print("Brake Actuation:", output_value)

# Visualize the fuzzy membership functions and rules
vehicle_speed.view()
brake_pressure.view()
brake_actuation.view()

# Display the plots
plt.show()
