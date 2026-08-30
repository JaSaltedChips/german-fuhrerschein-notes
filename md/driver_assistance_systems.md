# Driver Assistance Systems (Fahrerassistenzsysteme)

---

## Lane-Keep Assistance vs Lane-Change Assistance

| | Lane-Keep Assist | Lane-Change Assist |
|---|---|---|
| Driver's intention | Stay in lane | Move to another lane |
| Problem it prevents | Unintentional drift | Collision during intentional lane change |
| Sensors used | Camera (lane markings) | Radar (adjacent vehicles) |
| When it activates | Drifting without indicating | Indicating while blind spot is occupied |

---

## Lane Change Assist (Spurwechselassistent)

Monitors blind spots alongside and behind the vehicle using radar or cameras.

- Activates when the turn signal is used
- Warns if a vehicle is in or approaching the blind spot (visual in mirror, audible, or haptic)
- **Warning only — does not perform a lane change**
- Driver remains in full control at all times

### Without Steering Override
- Warnings still active
- System applies **no corrective steering** — driver can change lanes freely with no physical resistance

### Active Lane Change Assist (Aktiver Spurwechselassistent)

A more advanced variant that actually steers the vehicle into the adjacent lane:

1. Overall driver assistance system (typically ACC) must be active
2. Driver initiates by holding the indicator
3. System checks blind spots and adjacent lane
4. If clear, system automatically steers into the adjacent lane
5. Driver must keep hands on wheel and can override at any time

- Only works at certain speeds (typically motorway speeds)
- Driver **initiates** the manoeuvre — system does not decide independently
- Driver remains **legally responsible** at all times

---

## Cruise Control (Tempomat)

- Maintains a **set speed** chosen by the driver
- Does **not react** to other vehicles or traffic conditions
- If a vehicle ahead slows down, the system continues at the set speed — driver must brake manually
- Simple speed-holding only — no surrounding awareness

---

## Adaptive Cruise Control / ACC (Abstandsregeltempomat)

- Maintains a set speed **and** a set following distance to the vehicle ahead
- Uses **radar sensors** to detect the vehicle ahead
- Automatically **brakes** when the vehicle ahead slows down
- Automatically **accelerates** back to set speed when the way is clear
- Controls **longitudinal** movement only — **does not steer** and **does not perform lane changes**

### Cruise Control vs ACC

| Feature | Cruise Control | Adaptive Cruise Control |
|---|---|---|
| Maintains set speed | Yes | Yes |
| Reacts to vehicle ahead | No | Yes |
| Automatically brakes | No | Yes |
| Automatically accelerates | No (holds set speed only) | Yes |
| Sensors | None | Radar/camera |
| Steers the vehicle | No | No |

---

## Highway Assist / Pilot Assist

Combines ACC + lane centering and can semi-autonomously initiate lane changes.

- Activates turn signal → system checks surroundings → executes lane change if safe
- **Level 2 driver assistance** — driver must remain attentive and ready to take over at all times

---

## Lane Keeping Assist Systems (Spurhalteassistent)

Use a **front-facing camera** to detect lane markings. Do **not activate** if the turn signal is used — system assumes intentional lane change.

### 1. Lane Departure Warning (LDW) — Spurverlassenswarnung
- Warning only — no steering input
- Alerts when the vehicle crosses a lane marking without signaling
- Warning types: visual (dashboard), audible (beep), or haptic (steering wheel vibration)

### 2. Lane Keeping Assist (LKA) — Spurhalteassistent
- Warning + light corrective steering
- Applies brief steering torque to guide the vehicle back into the lane
- Driver can override easily by steering against it
- Reacts **after** the vehicle begins drifting

### 3. Lane Centering Assist — Spurmittenführung
- Continuous steering support
- Actively keeps the vehicle centered in the lane at all times
- Works in conjunction with ACC — forms the basis of **Highway Assist / Pilot Assist**
- Reacts **proactively**, not just when drifting occurs

### Summary

| System | Warning | Corrective Steering | Continuous? |
|---|---|---|---|
| Lane Departure Warning | Yes | No | No |
| Lane Keeping Assist | Yes | Yes (reactive) | No |
| Lane Centering Assist | — | Yes (proactive) | Yes |

---

## eCall (Emergency Call System)

Pan-European automatic emergency call system. Mandatory in all new passenger cars and light vans in the EU since **April 2018**.

When triggered, automatically calls **112** and transmits data to the nearest emergency call center (PSAP). A voice channel opens so occupants can speak with emergency services.

### Activation

| Method | How |
|---|---|
| **Automatic** | Crash sensors detect a severe impact (e.g. airbag deployment) — triggers without human action |
| **Manual** | Occupant presses the dedicated **SOS button** in the vehicle |

### Data Transmitted (Minimum Set of Data / MSD)

- GPS location and direction of travel
- Time of the incident
- Vehicle identification (VIN)
- Fuel type
- Whether activation was automatic or manual

### Key Points

- Uses the **mobile network** (GSM/4G) to connect
- Works even if occupants are unconscious (automatic mode)
- Transmits location **only at the moment of impact** — no ongoing tracking
- Mandatory in EU for new vehicles since **April 2018**

---

## Electronic Stability Program (ESP / ESC)

Detects and corrects loss of vehicle control — skidding, oversteer, or understeer — without driver input. Mandatory in all new passenger cars in the EU since **November 2011**.

### How it works

Continuously compares:
- **Intended direction** — steering angle sensor
- **Actual direction** — yaw rate sensor + lateral acceleration sensor

If a discrepancy is detected, ESP intervenes by selectively **braking individual wheels** and/or **reducing engine torque**. It does **not steer** the vehicle.

| Situation | Intervention |
|---|---|
| **Oversteer** (rear slides out) | Brakes the outer front wheel |
| **Understeer** (front washes out) | Brakes the inner rear wheel |

### Sensors Used
- Steering angle sensor
- Yaw rate sensor
- Wheel speed sensors (one per wheel)
- Lateral acceleration sensor

### Sub-systems within ESP
- **ABS** — Anti-lock Braking System (Antiblockiersystem)
- **TCS/ASR** — Traction Control (Antriebsschlupfregelung)
- **EBD** — Electronic Brake Distribution

### Warning Light

| Light behaviour | Meaning |
|---|---|
| **Flashing** | ESP is actively intervening — normal, temporary |
| **Continuously illuminated** | ESP is inactive — manually switched off or system fault |

If continuously illuminated and not manually deactivated: **have the vehicle checked** — ABS and traction control may also be affected.

---

## Limitations of Driver Assistance Systems

No system independently maintains all safety distances in all situations. Known limitations:

| Situation | Limitation |
|---|---|
| Stationary vehicles | Older ACC systems may not detect them |
| Poor weather (fog, rain, snow) | Sensors are impaired |
| Sharp bends | Vehicle ahead may leave sensor range temporarily |
| Motorcycles, cyclists, pedestrians | Detected less reliably than cars |
| Very slow speeds | Some systems disengage below a minimum speed |
| Emergency braking | System may not react fast enough |
| Road works / unusual layouts | System may behave unpredictably |

---

## Key Principles (StVO)

- The **driver** is always responsible for initiating and safely completing a lane change (StVO §7)
- No assistance system removes the driver's legal responsibility for their actions
- Driver must **continuously monitor** the system and be **ready to intervene** at all times
- Assistance systems are **aids**, not replacements for the driver
