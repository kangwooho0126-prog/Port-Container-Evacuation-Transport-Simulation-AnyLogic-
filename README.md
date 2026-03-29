#  Port Container Evacuation & Transport Simulation (AnyLogic)

##  Project Overview

This project develops a high-fidelity simulation model for port container transportation and emergency evacuation under high-load conditions using AnyLogic.

The system models the end-to-end container flow, including unloading, yard storage, and internal transport, to evaluate system performance and identify operational bottlenecks.

---

##  Demo

###  Quick Preview
![simulation](demo_simulation.gif)

###  Full Simulation Video
Watch full demo here:  
 (Put your Bilibili link here)

---

##  Problem Definition

In large-scale port operations, especially under emergency conditions (e.g., extreme weather or safety risks), all containers must be evacuated within a limited time window.

This problem involves:

- High container volume (up to ~35,000 TEU)
- Limited transport resources (trucks, cranes)
- Complex yard structure and road network
- Strong coupling between equipment and transport operations

 Objective:

- Minimize total evacuation time  
- Avoid congestion and system deadlock  
- Improve resource allocation efficiency  

---

##  System Modeling

The simulation is built using **AnyLogic (Discrete Event + Agent-based modeling)**.

### Key Components:

- **Yard System**  
  Block–Bay–Row–Tier structure for container storage

- **Transport Network**  
  Road topology with dynamic speed constraints

- **Resources**  
  - Quay cranes (STS)  
  - Yard cranes (RTG/RMG)  
  - Container trucks  
  - Operators  

- **Constraints**  
  - Speed limits (yard vs road)  
  - Turning radius (16.5m for trucks)  
  - Yard capacity and density  
  - Equipment handling rates  

---

##  Simulation Logic

The system simulates the following workflow:

1. Container unloading from vessels  
2. Transfer to yard via cranes  
3. Assignment to transport vehicles  
4. Movement through port road network  
5. Delivery to target evacuation yards  

Transport and handling processes are modeled with queueing, routing, and resource allocation logic.

---

##  Strategies

Two scheduling strategies are implemented and compared:

- **Dynamic Allocation Strategy**  
  Flexible assignment of transport resources

- **Priority-based Dispatching Strategy**  
  Containers dispatched based on predefined priority rules

---

##  Results & Insights

Simulation experiments show:

- Total evacuation time ranges from **15 to 31.7 days**, depending on container volume  
- **Transport fleet size is the most critical factor** affecting system performance  
- Increasing trucks significantly reduces evacuation time  
- **Diminishing returns** appear when fleet size exceeds a threshold  
- Major congestion occurs in **yard-to-road transition areas**

---

## Key Contributions

- Built a realistic port transport simulation system using AnyLogic  
- Modeled complex interactions between yard, transport, and equipment  
- Identified system bottlenecks through simulation experiments  
- Provided insights for **resource allocation and evacuation planning**

---

##  Project Structure
anylogic-port-simulation-model/
├── README.md
├── demo_simulation.gif
├── model/
│ └── port_model.alp
├── docs/
│ ├── system_design.png
│ ├── yard_structure.png
├── results/
│ └── simulation_results.png

---

##  Future Work

- Integrate optimization algorithms (e.g., vehicle routing, scheduling optimization)  
- Combine simulation with machine learning for adaptive decision-making  
- Extend to real-time digital twin applications  

---

##  Keywords

Supply Chain | Port Logistics | Simulation | AnyLogic | Scheduling | Transportation | Operations Research
