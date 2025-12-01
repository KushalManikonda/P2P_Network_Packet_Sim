# 🚀 Enhanced Network Routing Simulator

An interactive, browser-based network simulator that visualizes routing algorithms, packet flow, file transfers, and real-time topology modifications. This tool makes complex networking concepts more intuitive by combining simulation, animation, and editable graph topologies.

---

## 📁 Project Structure

```
📦 Enhanced-Network-Simulator
│
├── app.py                     # Backend server + WebSocket communication
├── network_topology.py        # Business logic: routing, nodes, packets
├── index.html                 # Frontend UI & visualization layer
└── README.md                  # Documentation
```

---

## 🌟 Features

- 🧭 **Multiple Routing Algorithms:** Shortest Path, BFS, Flooding, Link-State, Random Routing, BGP-style policy.
- 🔁 **Real-time Packet Animation:** Live hop-by-hop transfer with weight-based timing.
- ✨ **Editable Topology:** Add/delete nodes & links, drag reposition, live updates.
- 📦 **Simulated File Transfer:** Chunked transmission + parallel pipeline.
- 📡 **WebSocket Sync:** Backend and UI update instantly.
- 📜 **Activity Logging:** Routing decisions, delivery status, and simulation events.

---

## 🧩 Backend Modules

| Module | Description |
|--------|------------|
| `Network` Class | Maintains graph structure, nodes, and links |
| `Node` Class | Represents routers, switches, and hosts |
| `Packet` Class | Tracks metadata like TTL, hops, timestamps |
| Routing Endpoints | Handles routing requests and returns paths |
| Topology Endpoints | Add/remove nodes and edges dynamically |
| WebSocket Handlers | Emit live simulation events to frontend |
| File Transfer Handler | Splits files, transmits chunks, and reconstructs output |

---

## ⚙️ Business Logic Modules

| Module / Component | Role |
|-------------------|------|
| Dijkstra Algorithm | Weighted shortest path routing |
| BFS Engine | Hop-based route discovery |
| Flooding Logic | Broadcast routing simulation |
| Random Routing | Probabilistic next-hop routing |
| Link-State Router | Table generation similar to OSPF |
| BGP-Like Policy Routing | Hierarchical priority-based decisions |
| Packet Simulation Engine | Manages delay, TTL, reroute, and hop logic |
| File Chunk Scheduler | Manages parallel chunk transfers and assembly |

---

## 🎨 Frontend Modules  
(From UI in **index.html**)  
📄 *Source cited from uploaded HTML*

| Component | Purpose |
|----------|---------|
| Control Panel | Select routing method, nodes, transfer mode |
| Topology Editor | Add/remove nodes & links, drag reposition |
| Canvas Renderer | Draws graph with weights and device icons |
| Packet Animation System | Moves packets along route with timings |
| Route Formatter | Converts returned paths to visual labels |
| File Transfer UI | Upload, chunk settings, and execution |
| Activity Log | Shows routing paths, link weights, status updates |
| WebSocket Listener | Syncs backend events with UI visuals |

---

## ▶️ Installation & Running

### **1️⃣ Install Dependencies**

```bash
pip install flask flask-socketio
```

---

### **2️⃣ Start Backend Server**

```bash
python app.py
```

---

### **3️⃣ Open Frontend in Browser**

Visit:

```
http://localhost:5000
```

---

## 🧪 Example Use Cases

- Teaching routing concepts in networking labs  
- Comparing algorithm efficiency using visual metrics  
- Demonstrating dynamic network reconfiguration  
- Simulating file transfer routing behavior  

---

## 🔮 Future Enhancements

- 🔧 QoS-aware routing  
- 🌐 Multi-client shared simulation mode  
- 📈 Graph-based analytics dashboard  
- 🕸 Protocol extensions (TCP congestion control, UDP simulation)  
- 💾 Save & import topologies  

---

## 📄 License

This project is open for **research, learning, and non-commercial use**.

---

## 🙌 Credits

Designed for students, educators, and networking enthusiasts who want to *see* networks — not just configure them.

---

