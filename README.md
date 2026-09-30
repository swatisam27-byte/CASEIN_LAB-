# CASEIN_LAB-
Interactive Web-Based Virtual Lab for simulating casein extraction from milk using 3D visualization, real-time pH/temperature monitoring, titration, filtration, washing, and weighing.
🧪 Interactive 3D virtual laboratory for casein extraction using Three.js.

# 🧪 CaseinLab XR

### Interactive 3D Virtual Laboratory for Casein Extraction

**CaseinLab XR** is an interactive web-based virtual laboratory that simulates the process of **isolating casein from milk at its isoelectric point (pH 4.6)**.

The project provides a visual and interactive laboratory environment where users can perform the major steps of casein extraction, including **measuring milk, heating, acid titration, stirring, precipitation, filtration, washing, drying, and weighing**.

The laboratory is developed using **HTML, CSS, JavaScript, and Three.js**, with real-time simulation of temperature, pH, acid addition, precipitation, and experimental results.

---

## 🎯 Objectives

* Create an interactive virtual laboratory for casein extraction.
* Simulate the experimental procedure in a 3D environment.
* Demonstrate the effect of temperature and pH on casein precipitation.
* Provide real-time feedback during the experiment.
* Simulate filtration, washing, drying, and weighing.
* Calculate casein yield and recovery.
* Provide an experimental performance report.
* Support a two-user laboratory partner mode.
* Provide optional WebXR/VR support for compatible devices.

---

## 🔬 Experiment

The simulation is based on the isolation of casein from milk by bringing the milk close to its **isoelectric point of approximately pH 4.6**.

The simulated workflow is:

```text
Measure Milk
     ↓
Heat to 40°C
     ↓
Add Acetic Acid Dropwise
     ↓
Stir the Mixture
     ↓
Casein Precipitation
     ↓
Filter the Curds
     ↓
Wash with Water
     ↓
Wash with Ethanol
     ↓
Dry the Residue
     ↓
Weigh Casein
     ↓
Generate Report
```

---

## ✨ Features

### 🥛 Milk Measurement

Users can adjust the milk volume using an interactive graduated cylinder and transfer the selected volume into the beaker.

### 🌡️ Temperature Control

The virtual hot plate allows the user to control heating.

The experiment requires approximately:

**40 ± 2 °C**

The current temperature is displayed in real time.

### 🧪 Acid Titration

Users can add **10% acetic acid** dropwise.

The simulation provides controls for:

* Acid flow rate
* Drops per second
* Continuous acid addition

### 🔄 Stirring

The stirring intensity can be adjusted during titration.

Proper stirring affects the uniformity of precipitation.

### ⚗️ pH Monitoring

The interface displays the current pH value and provides a visual pH curve.

The simulation targets the casein isoelectric point:

**pH ≈ 4.6**

### 🥣 Casein Precipitation

As the experimental conditions approach the required temperature and pH, visible casein precipitation occurs inside the beaker.

The interface displays the percentage of precipitate formed.

### 🧻 Filtration

After sufficient precipitation, the user can filter the mixture to separate the casein curds from whey.

### 💧 Washing

The precipitated casein can be washed using:

* Water
* Ethanol

The washing process contributes to the simulated purity of the final product.

### ⚖️ Digital Balance

After washing and drying, the casein can be transferred to a virtual digital balance.

The simulated mass is displayed in grams.

### 📊 Experimental Report

At the end of the experiment, the application generates a report containing:

* Milk weight
* Dry casein mass
* Casein yield
* Recovery compared with theoretical yield
* Temperature control
* Mixing evenness
* Purity
* Peak precipitation
* Overall experimental score

### 👥 Partner Mode

The project includes a **Lab Partner Mode**.

Two browser tabs can be used simultaneously:

**Partner A**

* Controls heating

**Partner B**

* Controls acid addition and stirring

The two tabs communicate using the browser's **BroadcastChannel API**.

### 🥽 WebXR / VR Support

The project includes optional WebXR support for compatible browsers and VR devices.

The VR interface can be activated when immersive VR is supported by the browser.

---

## 🖥️ Technologies Used

| Technology           | Purpose                              |
| -------------------- | ------------------------------------ |
| HTML5                | Web page structure                   |
| CSS3                 | User interface and styling           |
| JavaScript           | Simulation logic and interaction     |
| Three.js             | 3D laboratory environment            |
| WebGL                | 3D rendering                         |
| WebXR                | Optional VR support                  |
| Canvas API           | pH graph and digital balance display |
| BroadcastChannel API | Partner mode communication           |

---

## 📁 Project Structure

The project can be kept as a single HTML file:

```text
CaseinLab-XR/
│
└── index.html
```

The HTML file contains:

* HTML structure
* Embedded CSS
* Embedded JavaScript
* Three.js integration

---

## 🚀 How to Run

### Method 1 — Directly in Browser

1. Download or clone the repository.
2. Open the project folder.
3. Open `index.html` in a modern web browser.
4. Select **Solo** to start the experiment.

### Method 2 — Using VS Code

1. Open the project folder in VS Code.
2. Open `index.html`.
3. Use a local development server such as **Live Server**.
4. Open the generated local URL in your browser.

> An internet connection is required when using the CDN version of Three.js included in the project.

---

## 🎮 How to Use

### Step 1 — Measure Milk

Adjust the graduated cylinder to the required volume and click:

**Pour into beaker**

The default target volume is:

**20 ml**

---

### Step 2 — Heat

Increase the hot plate power and allow the milk to reach approximately:

**40 ± 2 °C**

The system automatically advances once the required temperature is maintained.

---

### Step 3 — Add Acetic Acid

Use the titration controls to add acetic acid gradually.

Adjust:

* Drops/sec
* Stirring intensity

The objective is to approach the casein isoelectric point.

---

### Step 4 — Observe Precipitation

As the pH approaches approximately **4.6**, casein precipitation increases.

The simulation visually represents the formation of curds.

---

### Step 5 — Filter

Once curd formation is sufficient, click:

**Filter through paper**

The virtual beaker moves to the filtration setup.

---

### Step 6 — Wash

Wash the residue using:

**Water → Ethanol**

Both washing stages contribute to the simulated purity.

---

### Step 7 — Dry and Weigh

Place the residue on the digital balance.

The final simulated casein mass is displayed.

---

### Step 8 — View Report

After weighing, the application generates an experimental report containing the calculated results and performance metrics.

---

## 📊 Simulation Parameters

The application tracks several experimental variables:

```text
Temperature
pH
Milk Volume
Acid Volume
Stirring
Acid Flow Rate
Precipitation
Impurities
Purity
Temperature Control
Mixing Evenness
```

These variables interact to produce the final simulated casein yield.

---

## ⚠️ Experimental Feedback

The simulation provides feedback when experimental conditions are not ideal.

For example, adding acid too quickly without sufficient stirring can result in:

* Uneven precipitation
* Increased simulated impurities
* Reduced experimental performance

This allows students to understand how experimental technique can affect the final result.

---

## 🧮 Yield Calculation

The simulation estimates milk weight from the selected milk volume:

```text
Milk Weight = Milk Volume × 1.03
```

The theoretical casein content used by the simulation is approximately:

```text
2.6% of milk weight
```

The final report calculates:

```text
Yield = Dry Casein / Milk Weight × 100
```

and also provides recovery relative to the theoretical value.

---

## 🏆 Performance Score

The simulation generates an overall score based on several experimental factors, including:

* Precipitation quality
* Temperature control
* Mixing
* Purity
* Milk volume accuracy

The score is displayed after the experiment is completed.

---

## 👥 Lab Partner Mode

CaseinLab XR supports collaborative experimentation using two browser tabs.

### Partner A — Heating

Controls:

```text
Hot plate
Temperature
```

### Partner B — Acid + Stirring

Controls:

```text
Acid addition
Acid flow
Stirring
```

The tabs communicate using:

```javascript
BroadcastChannel
```

This creates a simple collaborative virtual laboratory experience without requiring a backend server.

---

## 🥽 VR Support

The application checks whether the browser supports:

```text
immersive-vr
```

If supported, a **VR** button becomes available.

The laboratory scene can then be viewed in a compatible VR environment.

---

## 🌐 Browser Compatibility

The project is intended for modern browsers supporting:

* WebGL
* JavaScript ES6+
* Canvas API
* BroadcastChannel API
* WebXR for VR functionality

Chrome or another modern Chromium-based browser is recommended for the best experience.

---

## 🔮 Future Improvements

Possible future enhancements include:

* 🔬 More detailed molecular visualization of casein precipitation
* 🧪 Additional milk/protein experiments
* 📈 Advanced experiment graphs
* 💾 Saving experiment results
* 👤 User accounts
* 🏫 Teacher/student dashboard
* 📝 Automatic lab reports
* 🌐 Multiplayer laboratory sessions
* 🥽 Improved VR interaction
* 📱 Better mobile controls
* 🎓 Experiment tutorials and quizzes
* 🔊 Audio instructions and laboratory feedback

---

## 🎓 Educational Purpose

CaseinLab XR is designed as an **educational virtual laboratory** that helps students understand the practical procedure and underlying variables involved in casein isolation.

Instead of performing the experiment only through theoretical instructions, students can interact with a simulated laboratory environment and observe how changing experimental conditions affects the outcome.

---

## 📜 License

This project is intended for educational and academic use.

You may modify and extend the project for learning and demonstration purposes.

---

## 👨‍💻 Project

**Project Name:** CaseinLab XR
**Type:** Interactive Virtual Laboratory
**Domain:** Educational Technology / Virtual Lab / 3D Web Application
**Primary Technologies:** HTML5, CSS3, JavaScript, Three.js, WebXR
