# Parcel-Collection-Simulation

ABM SETUP

    📦 Parcel Hub Simulation — Setup Guide
    
    This section explains how to configure and run the Parcel Hub Simulation model in NetLogo.
    
    🖥️ 1. World Setup
    
    The model uses a custom world size to represent the parcel hub layout:
    
    min-pxcor: –29
    
    max-pxcor: 30
    
    min-pycor: –9
    
    max-pycor: 10
    
    World wraps horizontally: ✔
    
    World wraps vertically: ✔
    
    Patch size: 15
    
    Frame rate: 30 FPS
    
    This custom world allows enough space to display the waiting area, service counter, walking paths, and exit points.
    
    🧩 2. Interface Layout
    
    The interface contains several key components:
    
    Buttons
    
    setup
    Initializes the world, clears all agents, resets variables, and prepares the environment for a new simulation.
    
    go
    Runs the simulation continuously.
    Inside go, the model:
    
    Generates customers
    
    Moves customers through the system
    
    Handles service logic
    
    Updates waiting statistics
    
    Increments simulation ticks
    
    🎛️ 3. Adjustable Parameters
    
    You can control the model using three sliders:
    
    1. mean-arrival-rate
    
    Controls how frequently new customers appear.
    
    Lower values → slower arrivals
    
    Higher values → busier queue
    
    2. mean-service-time
    
    Determines how long it takes for a clerk to serve one customer.
    
    Larger values → slower service
    
    Smaller values → faster service
    
    3. renege-probability
    
    The probability that a waiting customer will give up and leave.
    
    Represents impatience or frustration due to long queues.
    
    🔢 4. Monitors
    number-of-customer-waiting
    
    Displays the current number of customers who are waiting to be served.
    
    This value updates every tick based on the number of customers not currently being served.
    
    🧱 5. World Layout (Colored Areas)
    
    The simulation interface includes visual areas:
    
    Blue region — overall parcel hub area
    
    Green bars — benches or waiting zones
    
    Pink rectangle — service counter
    
    Gray vertical bars — pathways or queue lanes
    
    These areas guide customer movement and seating behavior.
    
    ▶️ 6. Running the Model
    
    Click setup
    
    Resets world
    
    Places benches, service counter, and paths
    
    Resets clerk state and timers
    
    Adjust sliders (arrival rate, service time, renege probability)
    
    Click go
    
    Customers begin arriving
    
    They walk, sit, queue, renege, get served, and exit
    
    The counter updates automatically
    
    Observe how queue length and service speed affect the system.
