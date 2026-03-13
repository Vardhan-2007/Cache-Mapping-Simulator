# Cache-Mapping-Simulator
Project for my academics subject Computer Organisation and Micro Processors

# 🧠 Cache Mapping Simulator (COA)

An interactive **web-based simulator** to visualize how different **cache mapping techniques** work in **Computer Organization & Architecture (COA)**.

This project helps students understand **Direct Mapping, Fully Associative Mapping, and Set-Associative Mapping** through **step-by-step simulation, cache visualization, hit/miss tracking, and performance graphs**.

---

# 🚀 Features

- Interactive cache visualization
- Step-by-step simulation
- Auto play simulation
- Hit / Miss tracking
- Hit ratio and miss ratio calculation
- Real-time performance graph
- CSV export of simulation results
- LRU replacement policy support
- Clean and modern UI

---

# 📚 Cache Mapping Techniques Implemented

## 1️⃣ Direct Mapping

Each memory block maps to **exactly one cache line**.

**Formula**

```
Cache Line = Address % Cache Size
```

**Characteristics**

- Simple and fast
- Low hardware cost
- Higher conflict misses

---

## 2️⃣ Fully Associative Mapping

Any memory block can be stored in **any cache line**.

**Characteristics**

- Highest flexibility
- Better hit ratio
- Requires replacement algorithms

**Replacement Policies**

- FIFO
- LRU (toggle option available)

---

## 3️⃣ Set-Associative Mapping

A hybrid approach between **Direct Mapping** and **Fully Associative Mapping**.

Cache is divided into **sets**, and each set contains multiple **ways**.

**Formula**

```
Set Index = Address % Number of Sets
```

**Characteristics**

- Balanced performance
- Used in real CPU caches
- Supports LRU replacement

---

# 🖥️ Project Interface

## 🏠 Home Page

Allows users to select the cache mapping technique:

- Direct Mapping
- Fully Associative Mapping
- Set Associative Mapping

---

# ⚙️ Simulation Controls

| Control | Description |
|------|------|
| Addresses | Memory address sequence |
| Cache Size | Number of cache lines |
| Block Size | Memory block size |
| Ways | Number of blocks per set (Set-Associative only) |
| Speed | Simulation playback speed |
| Start | Initialize simulation |
| Next | Execute next step |
| Play | Auto run simulation |
| Reset | Reset simulator |
| Export CSV | Download simulation results |
| Home | Return to main page |

---

# 📊 Statistics Displayed

The simulator tracks:

- Current address
- Cache hits
- Cache misses
- Hit ratio
- Miss ratio
- Cache state visualization
- Performance graph

---

# 📈 Visualization

The simulator provides:

- Cache block visualization
- Green highlight → Cache Hit
- Red highlight → Cache Miss
- Real-time hit ratio graph using Canvas API

---

# 📁 Project Structure

```
Cache-Mapping-Simulator
│
├── index.html
├── direct.html
├── fully.html
├── set.html
│
└── README.md
```

**Files Description**

| File | Purpose |
|-----|-----|
| index.html | Home page to select mapping technique |
| direct.html | Direct Mapping simulator |
| fully.html | Fully Associative simulator |
| set.html | Set Associative simulator |

---

# 🛠️ Technologies Used

- HTML5
- CSS3
- Vanilla JavaScript
- Canvas API for graph visualization

No external libraries or frameworks are used.

---

# ▶️ How to Run

## Method 1 — Open Directly

1. Download or clone the repository
2. Open the file

```
index.html
```

in your web browser.

---

## Method 2 — Run with Local Server

Example using Python:

```
python -m http.server 8000
```

Open in browser:

```
http://localhost:8000
```

---

# 📥 Example Address Sequence

Example input:

```
0,1,2,3,0,1,4,0,1,2,3,4
```

You can experiment with different:

- Cache sizes
- Block sizes
- Number of ways
- Address sequences

---

# 📤 Export Results

Simulation results can be exported as **CSV file**.

Example output:

```
step,address,result
1,0,MISS
2,1,MISS
3,2,MISS
4,3,MISS
5,0,HIT
...
```

This is useful for:

- Lab reports
- Performance analysis
- COA assignments

---

# 🎓 Educational Use

This simulator is useful for learning:

- Computer Organization
- Cache Memory
- Memory Hierarchy
- Cache Replacement Algorithms

Suitable for:

- B.Tech students
- Computer Science learners
- COA laboratory demonstrations

---

# ⭐ Future Improvements

Possible enhancements:

- Cache address breakdown (Tag / Index / Offset)
- Multi-level cache simulation (L1, L2, L3)
- Visual memory block diagrams
- Additional replacement algorithms
- Performance comparison between mapping techniques
- React-based UI

---

# 👨‍💻 Author

**Vardhan**

B.Tech – Artificial Intelligence & Machine Learning

Interests:

- Computer Architecture
- AI/ML Development
- System Design
- ISRO / DRDO Research Technologies

---

## Note

This project was developed as a personal learning project and is shared for educational purposes.
