# 🅿️ Smart Parking System

A comprehensive **Java-based Smart Parking Management System** that efficiently manages parking slots, vehicles, and revenue using advanced **Data Structures**.

## 📋 Table of Contents
- [Features](#features)
- [Technology Stack](#technology-stack)
- [Data Structures Used](#data-structures-used)
- [Project Structure](#project-structure)
- [Installation & Setup](#installation--setup)
- [Usage](#usage)
- [Example Output](#example-output)
- [Author](#author)

---

## ✨ Features

✅ **Vehicle Parking Management** - Efficiently park and unpark vehicles  
✅ **Real-time Slot Availability** - Check available parking slots instantly  
✅ **Automated Fee Calculation** - Calculate parking fees based on duration  
✅ **Vehicle Tracking** - Find vehicle location in the parking lot  
✅ **Occupancy Monitoring** - View real-time parking occupancy rate  
✅ **Recently Freed Slots** - Track recently freed slots using Stack  
✅ **Parking History** - Maintain complete history of all vehicles  
✅ **Revenue Management** - Calculate total parking revenue  
✅ **Multi-type Slots** - Support for Standard and Premium slots  

---

## 🛠️ Technology Stack

| Technology | Purpose |
|-----------|---------|
| **Java** | Core programming language |
| **Object-Oriented Programming** | Class-based design (Vehicle, ParkingSlot) |
| **Data Structures** | ArrayList, HashMap, Queue, Stack, LinkedList |
| **DateTime API** | Track entry/exit times |

---

## 📊 Data Structures Used

1. **ArrayList** 
   - Stores all parking slots dynamically
   - Allows efficient slot management and traversal
   - Time Complexity: O(1) for access

2. **HashMap**
   - Maps Vehicle IDs to Vehicle objects
   - Enables O(1) lookup time for finding vehicles
   - Key: Vehicle ID, Value: Vehicle object

3. **Queue (LinkedList)**
   - Manages vehicles exiting the parking system
   - FIFO (First In First Out) principle
   - Used for exit processing

4. **Stack**
   - Stores recently freed slot numbers
   - LIFO (Last In First Out) principle
   - Quick access to recently available slots

5. **LinkedList**
   - Maintains complete parking history
   - Efficient insertion at both ends
   - Time Complexity: O(1) for add/remove

---

## 📁 Project Structure

```
smart-parking-system/
│
├── SmartParkingSystem.java    # Main application
├── Vehicle.java               # Vehicle class
├── ParkingSlot.java          # Parking slot class
├── README.md                 # Documentation
└── LICENSE                   # License file
```

---

## 🚀 Installation & Setup

### Prerequisites
- Java Development Kit (JDK) 8 or higher
- Any IDE (IntelliJ IDEA, Eclipse, VS Code) or command line

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/tasmia-fatima/smart-parking-system.git
   cd smart-parking-system
   ```

2. **Compile the Java file**
   ```bash
   javac SmartParkingSystem.java
   ```

3. **Run the application**
   ```bash
   java SmartParkingSystem
   ```

---

## 💻 Usage

### Main Operations

#### 1. Park a Vehicle
```java
parkingSystem.parkVehicle("CAR-001", "Car", "Ali Ahmed");
```
- **Parameters**: Vehicle ID, Type (Car/Bike/Truck), Owner Name
- **Returns**: Boolean (success/failure)
- **Time Complexity**: O(n) - searches for available slot

#### 2. Unpark a Vehicle
```java
parkingSystem.unparkVehicle("CAR-001");
```
- **Calculates**: Parking duration and fee
- **Updates**: Total revenue
- **Returns**: Fee details

#### 3. Check Parking Status
```java
parkingSystem.getParkingStatus();
```
- Shows: Total, Occupied, Available slots
- Displays: Occupancy percentage

#### 4. Find Vehicle Location
```java
parkingSystem.findVehicle("CAR-001");
```
- Uses HashMap for O(1) lookup
- Returns: Vehicle location and details

#### 5. View Recently Freed Slots
```java
parkingSystem.viewRecentlyFreedSlots();
```
- Uses Stack data structure
- Shows: Last 5 freed slots

#### 6. View Parking History
```java
parkingSystem.viewParkingHistory();
```
- Uses LinkedList
- Shows: Complete entry/exit history

#### 7. Display Revenue
```java
parkingSystem.displayRevenue();
```
- Shows: Total revenue collected

---

## 📤 Example Output

```
═══════════════════════════════════════
  SMART PARKING SYSTEM - DEMO
═══════════════════════════════════════

✅ Parking System Initialized with 10 slots
✅ Vehicle Parked Successfully!
   Vehicle ID: CAR-001
   Slot: SLOT-1
   Time: 2024-01-15T10:30:45

📊 PARKING STATUS
   Total Slots: 10
   Occupied: 4
   Available: 6
   Occupancy Rate: 40.00%

✅ Vehicle Unparked Successfully!
   Vehicle ID: CAR-001
   Parked Duration: 0.03 hours
   Fee: PKR 1.50
   Slot: SLOT-1 is now FREE

💰 TOTAL REVENUE: PKR 500.00
```

---

## 🎯 Algorithms & Complexity Analysis

| Operation | Data Structure | Time Complexity | Space Complexity |
|-----------|-----------------|-----------------|------------------|
| Park Vehicle | ArrayList | O(n) | O(1) |
| Find Vehicle | HashMap | O(1) | O(n) |
| Unpark Vehicle | ArrayList + HashMap | O(n) | O(1) |
| Get Status | ArrayList | O(n) | O(1) |
| View History | LinkedList | O(1) per operation | O(n) |

---

## 🔄 Future Enhancements

- [ ] Database integration (MySQL/MongoDB)
- [ ] Web UI dashboard
- [ ] QR code-based vehicle identification
- [ ] Slot reservation system
- [ ] Mobile app development
- [ ] Payment gateway integration
- [ ] Real-time notifications
- [ ] Admin panel

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

---

## 👨‍💻 Author

**Tasmia Fatima**
- 🎓 BSCS Student at Air University
- 📧 Email: tasmiafatima42@gmail.com
- 🔗 LinkedIn: [linkedin.com/in/tasmia-fatimaa9a498390](https://linkedin.com/in/tasmia-fatimaa9a498390)
- 💻 GitHub: [github.com/tasmia-fatima](https://github.com/tasmia-fatima)

---

## 🌟 Show Your Support

Give a ⭐ if this project helped you!

---

**Made with ❤️ by Tasmia Fatima**
