## HDRI Manager

Professional HDRI workflow with color grading controls built-in.

### What is HDRI Manager?

Load and control HDRIs (environment textures) with advanced color correction:
- **Visual browser** with thumbnails
- **Temperature** control (warm/cool adjustment)
- **Tint** control (green/magenta adjustment)
- **One-click setup** with automatic node creation

---

### First-Time Setup

#### Configure HDRI Assets Folder

1. Download HDRIs (free from [Poly Haven](https://polyhaven.com/hdris))
2. Put all `.hdr` or `.exr` files in one folder
3. Open Blender `Preferences > Add-ons > Light Manager Pro`
4. **Set "HDRI Assets Folder"** to your folder path
5. Close preferences

✅ Now HDRI Manager can find your HDRIs!

---

### Loading an HDRI

#### Method 1: Grid Browser (Visual)

1. Open **"World & HDRI Manager"** section
2. Click **"Select HDRI from Grid"** button
3. **Grid popup appears** showing HDRI thumbnails
4. **Click on an HDRI** to load it
5. ✨ HDRI loads automatically with all controls!

#### What Happens Automatically:

- World shader nodes created
- HDRI loaded and connected
- Temperature/Tint node group added
- Mapping node for rotation
- Everything ready to adjust

---

### Adjusting HDRI

After loading, adjust in the **"Surface"** section:

#### Rotation

**Purpose**: Rotate HDRI to position sun/light sources

1. Find **"Rotation Z"** slider in Surface section
2. Drag slider to rotate HDRI around Z-axis
3. Range: -180° to +180°
4. Watch viewport update in real-time

**💡 Tip**: Use rotation to place HDRI sun behind your subject for rim lighting.

---

#### Strength

**Purpose**: Control HDRI brightness/intensity

1. Find **"Strength"** slider
2. Adjust to make HDRI brighter or dimmer
3. Typical ranges:
   - Interior scenes: 0.3 - 1.0
   - Outdoor scenes: 1.0 - 3.0
   - Studio: 0.5 - 1.5

**💡 Tip**: Lower strength for more control from your scene lights.

---

#### Temperature (Warm/Cool)

**Purpose**: Adjust color temperature without changing HDRI

**Range**: -1.0 (Warm/Orange) to +1.0 (Cool/Blue)

1. Find **"Temperature"** slider in Surface section
2. **Drag left** (negative) for warmer, orange tones
3. **Drag right** (positive) for cooler, blue tones
4. **Center (0.0)** = neutral, original HDRI colors

**Use Cases:**
- Golden hour: Temperature -0.5 to -0.8
- Cool winter: Temperature +0.3 to +0.6
- Neutral: 0.0

**💡 Pro Tip**: Combine with color management for precise looks.

---

#### Tint (Green/Magenta)

**Purpose**: Correct or add color casts

**Range**: -1.0 (Green) to +1.0 (Magenta)

1. Find **"Tint"** slider
2. **Drag left** (negative) for green tint
3. **Drag right** (positive) for magenta tint
4. **Center (0.0)** = neutral

**Use Cases:**
- Correct green color cast: Tint +0.2 to +0.5
- Alien atmosphere: Tint -0.6 (green)
- Warm studio: Tint +0.3 (magenta)

---

### HDRI Manager Best Practices

✅ **DO:**
- Organize HDRIs into subfolders by type (Studio, Outdoor, etc.)
- Use linear HDRIs (not tonemapped JPEGs)
- Start with Strength 1.0, adjust from there
- Use subtle Temperature/Tint (-0.3 to +0.3) for natural looks

❌ **DON'T:**
- Mix HDRIs from different sources without color matching
- Use extreme Temperature/Tint values (> ±0.8) unless stylized
- Forget to adjust rotation for best lighting angle

**💡 Workflow Tip:**
1. Load HDRI
2. Rotate to position main light source
3. Adjust Strength for desired intensity
4. Fine-tune Temperature for mood
5. Subtle Tint correction if needed

---
