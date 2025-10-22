## Lighting Scenarios System

Create, save, and manage multiple lighting setups in one scene.

### What are Lighting Scenarios?

Scenarios are **saved lighting configurations**. Instead of duplicating your entire scene for different lighting moods, you can:
- Save unlimited lighting setups in one file
- Switch between them instantly
- Blend scenarios together
- Animate transitions between scenarios

**Use Cases:**
- Archviz: Day/Night/Golden Hour lighting
- Product: Studio/Dramatic/Soft lighting variations
- Animation: Different times of day
- Presentations: Multiple lighting options for clients

---

### Creating Your First Scenario

#### Step 1: Set Up Your Lights

1. Create your scene with objects
2. Add lights and adjust them for your first lighting look
   - Example: "Studio Lighting" with soft, even lights
3. Adjust power, color, position until you're happy

#### Step 2: Save as Scenario

1. Open **Lighting Scenarios** section in the panel
2. Click **"Create New Scenario"** button
3. **Name your scenario** (e.g., "Studio")
4. Click **"Save Scenario"**

✅ Your first scenario is saved!

#### Step 3: Create a Second Scenario

1. **Modify your lights** for a different look
   - Change power, colors, add/remove lights
   - Example: "Dramatic" with harsh shadows
2. Click **"Create New Scenario"** again
3. Name it (e.g., "Dramatic")
4. Click **"Save Scenario"**

✅ Now you have two scenarios!

---

### Switching Between Scenarios

#### Method 1: Scenario List (Quick Switch)

1. Find your saved scenarios in the list
2. **Click on a scenario name**
3. ✨ Lights instantly update to that configuration!

**That's it!** Your lighting changes in real-time.

---

#### Method 2: Scenario Mode (Advanced)

**Scenario Mode** gives you a focused UI with more controls.

**To Enter Scenario Mode:**

1. Click **"Enter Scenario Mode"** button
2. Select a scenario from the dropdown
3. Your lights update
4. Panel shows special "Scenario Mode" UI

**What You Can Do in Scenario Mode:**
- Quick scenario switching
- See which scenario is active
- Access scenario-specific tools
- **Auto-tagging**: New lights automatically added to current scenario

**To Exit Scenario Mode:**

1. Click **"Exit Scenario Mode"** button
2. Returns to normal panel

**💡 Tip:** Use Scenario Mode when actively working on specific scenarios.

---

### Scenario Blending (A to B)

**Blend between two scenarios** for smooth transitions or in-between looks.

#### Step-by-Step: Create a Blend

1. Click **"Scenario Blend (A to B)"** section
2. **Select Scenario A**: Choose first scenario (e.g., "Day")
3. **Select Scenario B**: Choose second scenario (e.g., "Night")
4. Click **"Enter Blend Mode"**

#### Adjust the Blend

1. Use the **"Blend Factor"** slider
   - `0%` = 100% Scenario A
   - `50%` = Equal mix of A and B
   - `100%` = 100% Scenario B
2. **Lights update in real-time** as you drag the slider
3. Find the perfect in-between look

#### Save or Exit

**To Save the Blend as New Scenario:**
1. Click **"Save Current as New Scenario"**
2. Name it (e.g., "Sunset")
3. Now you have a permanent in-between scenario

**To Exit Blend Mode:**
1. Click **"Exit Blend Mode"**

**💡 Pro Tip:** Use blending to create variations without manual light adjustment!

---

### Multi-Scenario Mixer (Advanced)

**Mix multiple scenarios simultaneously** with individual weight control.

#### When to Use Mixer

- Combine 3+ scenarios
- Need precise control over each scenario's contribution
- Creating complex, layered lighting

#### Step-by-Step: Use the Mixer

1. Click **"Scenario Mixer"** section
2. Click **"Create Mixer Slot"**

#### Configure Mixer Slots

1. Each slot has:
   - **Scenario Selector**: Choose which scenario
   - **Weight Slider**: Control contribution (0.0 to 1.0)
2. Add multiple slots (up to 30 scenarios!)
3. Adjust weights for each

#### Examples

**Example 1: Time Blending**
- Slot 1: "Morning" (weight 0.3)
- Slot 2: "Noon" (weight 0.5)
- Slot 3: "Afternoon" (weight 0.2)
- **Result**: Custom time-of-day blend

**Example 2: Style Mixing**
- Slot 1: "Studio" (weight 0.6)
- Slot 2: "Dramatic" (weight 0.3)
- Slot 3: "Colorful" (weight 0.1)
- **Result**: Unique lighting style

#### Clear/Reset Mixer

1. Click **"Clear All Weights"** to reset everything to 0
2. Or delete individual slots

---

### Animation Helpers

**Keyframe transitions between scenarios** for animations.

#### Step-by-Step: Animate Scenario Transition

1. Go to **"Animation Helpers"** section
2. Click **"Add Blend Helper"**
3. **Configure the helper:**
   - **Name**: "Day to Night Transition"
   - **Scenario A**: "Day"
   - **Scenario B**: "Night"
   - **Blend Factor**: Start at 0.0

#### Create the Animation

1. **Frame 1**: Set Blend Factor to `0.0` (100% Day)
   - Hover over blend factor slider
   - Press `I` to keyframe
2. **Frame 120**: Move timeline to frame 120
   - Set Blend Factor to `1.0` (100% Night)
   - Press `I` to keyframe
3. **Play animation**: Smooth transition from day to night!

**💡 Tip:** Multiple animation helpers can run simultaneously for complex sequences.

---

### Scenario Tagging

**Organize lights** by assigning them to scenarios without duplication.

#### What is Scenario Tagging?

Instead of duplicating lights:
- **One light** can belong to **multiple scenarios**
- Each scenario remembers that light's settings
- Cleaner scene, less clutter

#### Step-by-Step: Tag Lights

1. **Select light(s)** in your scene
2. Go to **"Scenario Tagging"** section
3. Enter scenario name in **"Tag with Scenario"** field
4. Click **"Apply Tag"**

✅ Light is now tagged with that scenario!

#### View Tagged Lights

1. In Lights Hierarchy, tagged lights show scenario badges
2. Filter by scenario tag using **"Tag Filter"** dropdown

#### Multi-Scenario Lights

One light in multiple scenarios:
1. Select light
2. Tag with "Studio"
3. Tag same light with "Dramatic"
4. Light now belongs to both scenarios with different settings

---

### Managing Scenarios

#### Rename a Scenario

1. Find scenario in list
2. Click **rename icon** (pencil)
3. Enter new name
4. Press Enter

#### Delete a Scenario

1. Find scenario in list
2. Click **delete icon** (X)
3. Confirm deletion
4. ⚠️ This cannot be undone!

#### Update a Scenario

1. Modify lights in your scene
2. Select the scenario to update
3. Click **"Update Scenario"** button
4. Current light settings replace saved settings

---

### Scenario Best Practices

✅ **DO:**
- Use clear, descriptive names ("Studio_Soft", "Outdoor_Noon")
- Save often as you work
- Test switching before final renders
- Use tags for lights that appear in multiple scenarios

❌ **DON'T:**
- Create 50+ scenarios (gets messy - use variations instead)
- Delete scenarios without backups
- Forget to save changes before switching
- Mix scenario systems with manual light hiding

**💡 Workflow Tip:**
1. Create base scenarios first (Day, Night, Studio)
2. Use blending to create variations
3. Save successful blends as new scenarios
4. Use animation helpers for sequences

---
