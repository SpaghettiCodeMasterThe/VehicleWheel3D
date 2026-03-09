# VehicleWheel3D
Problem:
When the suspension compresses fully, the normal force becomes massive, and since friction is often calculated as $\text{Friction} = \mu \cdot F_n$, the grip becomes "infinite," causing the car to flip or stop instantly.

Solution: Download Godot source and replace vehicle_body_3d.cpp and vehicle_body_3d.h

Wheel Compressed Suspension Threshold: This is a distance in meters. If your Rest Length is 0.15 and your Travel is 0.1, the absolute minimum suspension length is 0.05. Set this threshold slightly higher than the minimum (e.g., 0.06) so it triggers just before bottoming out.

Wheel Compressed Friction Slip: Set this to something very low, like 0.2 or 0.5, so the tires immediately let go and slide upon impact.
