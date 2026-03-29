#  Port Container Evacuation & Transport Simulation (AnyLogic)

##  Project Overview

This project develops a high-fidelity simulation system for port container transportation and emergency evacuation using AnyLogic.

The model captures the full operational process, including container handling, yard storage, and internal transport, to evaluate system performance under large-scale scenarios.

---

##  Demo

![simulation_demo](port_transport_simulation_demo.gif)



---

##  Simulation Preview

### System Modeling (Process Flow)
![logic](simulation_logic.png)

### 3D Simulation Environment
![3d](port_3d_view.png)

---

##  Problem Definition

In large-scale port operations, especially under emergency scenarios, all containers must be evacuated within a limited time.

Key challenges include:

- High container volume (~35,000 TEU)
- Limited transport capacity (trucks, cranes)
- Complex yard structure and road network
- Strong coupling between handling equipment and transport system

---

##  System Modeling

The simulation is built using **AnyLogic (Discrete Event + Agent-based modeling)**.

### Key Components

- **Yard System**  
  Block–Bay–Row–Tier container storage structure

- **Transport Network**  
  Road topology with routing and congestion constraints

- **Resources**  
  - Container trucks  
  - Yard cranes  
  - Handling equipment  

- **Constraints**  
  - Speed limits in different zones  
  - Vehicle turning radius  
  - Yard capacity limits  
  - Resource availability  

---

##  Simulation Logic

The system simulates the full operational workflow:

1. Container generation / unloading  
2. Storage allocation in yard  
3. Transport assignment  
4. Vehicle routing through network  
5. Delivery to evacuation zones  

The model integrates queueing, routing, and resource scheduling mechanisms.

---

##  Strategies

Two strategies are implemented:

- **Dynamic Resource Allocation**  
- **Priority-based Dispatching**

---

##  Results & Insights

- Total evacuation time ranges from **15 to 31.7 days**
- Transport fleet size is the dominant factor
- Increasing vehicles significantly reduces completion time
- Diminishing returns appear beyond a threshold
- Bottlenecks mainly occur at **yard-road interfaces**

---

##  Modeling Highlights

- Transport scheduling with resource constraints  
- Dynamic routing with congestion effects  
- Coupled crane–vehicle operations  
- Simulation-based bottleneck identification  

---

##  Note

Due to confidentiality considerations, the full AnyLogic model and dataset are not publicly available.

However, system design, simulation results, and demonstrations are provided to illustrate the modeling and analysis process.

---

##  Keywords

Supply Chain | Port Logistics | Simulation | AnyLogic | Scheduling | Transportation | Operations Research
