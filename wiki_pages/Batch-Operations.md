## Batch Operations

Powerful tools for managing multiple lights simultaneously.

### What are Batch Operations?

Instead of editing lights one-by-one:
- **Select multiple lights**
- **Apply operations** to all at once
- **Save time** on repetitive tasks
- **Consistency** across lights

**Categories:**
- Color operations
- Power/Energy operations
- Organization operations
- Selection operations
- Visibility operations

---

### Batch Selection

**Select multiple lights quickly** before operations.

#### Select by Type

1. Go to **"Batch Operations"** section
2. **Click "Select by Type"** dropdown:
   - Area Lights
   - Point Lights
   - Spot Lights
   - Sun Lights
   - All Lights
3. All lights of that type are selected

#### Select by Name Pattern

**Select lights with similar names:**

1. Click **"Select by Name"**
2. Enter pattern (e.g., "Key_*" or "*_Fill")
3. Click **"Select"**
4. All matching lights selected

**Patterns:**
- `*` = any characters
- `Key_*` = Starts with "Key_"
- `*_Fill` = Ends with "_Fill"
- `*Light*` = Contains "Light"

#### Select by Collection

1. Click **"Select by Collection"**
2. Choose collection from dropdown
3. All lights in that collection selected

---

### Color Operations

#### Apply Color to All

**Set same color for multiple lights:**

1. **Select lights** (use batch selection)
2. Go to **"Color Operations"** subsection
3. **Choose color** using color picker
4. Click **"Apply Color"**

✅ All selected lights now have that color!

---

#### Randomize Colors

**Add variety to multiple lights:**

1. Select lights
2. Click **"Randomize Colors"**
3. **Options:**
   - Hue Range: How varied (0.0 = similar, 1.0 = full rainbow)
   - Saturation: How colorful (0.0 = white, 1.0 = vivid)
   - Value: How bright (0.0 = black, 1.0 = bright)
4. Click **"Randomize"**

**Result**: Each light gets a random color within your parameters.

---

#### Color Gradient

**Create smooth color transition across lights:**

1. Select lights in order (selection order matters!)
2. Click **"Color Gradient"**
3. **Set Start Color** (first light)
4. **Set End Color** (last light)
5. Click **"Apply Gradient"**

**Result**: Smooth color transition from first to last selected light.

**💡 Example**: Red → Orange → Yellow sunrise effect across 5 lights.

---

#### Color Ramp

**Apply color ramp from textures:**

1. Create color ramp texture (in Shader Editor)
2. Select lights
3. Click **"Apply Color Ramp"**
4. Choose texture from dropdown
5. Click **"Apply"**

**Result**: Each light samples a different point on the ramp.

---

### Power Operations

#### Adjust Power (All)

**Change energy for multiple lights:**

1. Select lights
2. Go to **"Power Operations"**
3. **Choose mode:**
   - **Set**: Replace power value
   - **Add**: Increase by amount
   - **Multiply**: Scale by factor
4. Enter value
5. Click **"Apply"**

**Examples:**
- Set all to 100W: Mode=Set, Value=100
- Increase all by 50W: Mode=Add, Value=50
- Double all: Mode=Multiply, Value=2.0
- Halve all: Mode=Multiply, Value=0.5

---

#### Randomize Power

**Add variation to light intensity:**

1. Select lights
2. Click **"Randomize Power"**
3. **Set range:**
   - Minimum: Lowest power value
   - Maximum: Highest power value
4. Click **"Randomize"**

**Example**: Min=50, Max=150 → Each light gets random value between 50-150W.

---

#### Power Distribution

**Evenly distribute power across lights:**

1. Select lights (e.g., 4 lights)
2. Click **"Distribute Power"**
3. **Enter total power** (e.g., 400W)
4. Click **"Distribute"**

**Result**: Each light gets equal share (4 lights × 100W = 400W total).

**💡 Use Case**: Ensure consistent illumination from multiple sources.

---

#### Clamp Power

**Limit power values within range:**

1. Select lights
2. Click **"Clamp Power"**
3. **Set limits:**
   - Min: Minimum allowed power
   - Max: Maximum allowed power
4. Click **"Clamp"**

**Result**: Lights below min are raised to min, above max are lowered to max.

**💡 Use Case**: Prevent overly dim or bright lights after randomization.

---

### Organization Operations

#### Auto-Organize by Prefix

**Create collections based on light name prefixes:**

1. Select lights (names like "Key_Light1", "Key_Light2", "Fill_Light1")
2. Click **"Organize by Prefix"**
3. Enter **separator character** (default: `_`)
4. Click **"Organize"**

**Result:**
- Collection "Key" created with Key_Light1, Key_Light2
- Collection "Fill" created with Fill_Light1

**💡 Naming Convention**: Use `Type_Description` format.

---

#### Auto-Organize by Suffix

**Same as prefix, but uses end of name:**

1. Select lights (names like "ProductA_Key", "ProductB_Key")
2. Click **"Organize by Suffix"**
3. Enter separator (default: `_`)
4. Click **"Organize"**

**Result**: Collection "Key" with both ProductA_Key and ProductB_Key.

---

### Visibility Operations

#### Show All Lights

**Make all lights visible in viewport:**

1. Click **"Show All Lights"** button
2. All lights in scene become visible

**💡 Use Case**: After hiding lights for cleaner viewport, show all again.

#### Hide All Lights

**Hide all lights in viewport:**

1. Click **"Hide All Lights"**
2. All lights hidden (still render!)

**💡 Use Case**: Clean up viewport while working on modeling/texturing.

**⚠️ Note**: Lights still render even when hidden in viewport.

---

### Batch Operations Best Practices

✅ **DO:**
- Select carefully before batch operations
- Use Undo (`Ctrl+Z`) if operation wasn't what you wanted
- Name lights consistently for easier batch selection
- Test on a few lights before applying to all
- Use batch operations for repetitive tasks

❌ **DON'T:**
- Apply batch operations without selecting (affects nothing)
- Forget you can Undo
- Batch modify lights in locked collections
- Use extreme randomization values (creates chaos)

**💡 Workflow Tips:**

**Quick Setup:**
1. Add multiple lights
2. Batch select by type
3. Apply base color
4. Randomize power slightly (±20%)
5. Organize into collections

**Maintenance:**
1. Select all lights
2. Clamp power (min=10, max=1000)
3. Organize by prefix
4. Save file

---
