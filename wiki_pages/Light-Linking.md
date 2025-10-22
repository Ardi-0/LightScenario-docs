## Light Linking

Control which lights affect which objects.

### What is Light Linking?

By default, all lights affect all objects. Light Linking lets you:
- **Link lights** to specific objects only
- **Exclude objects** from specific lights
- **Fine control** over complex scenes
- **Faster renders** (lights ignore irrelevant objects)

**Use Cases:**
- Product rendering: Separate rim light just for product
- Character lighting: Face light that doesn't affect background
- Archviz: Interior lights don't affect exterior
- Multi-object scenes: Different lighting per object

---

### Understanding Inclusion vs Exclusion

**Two Modes:**

1. **Inclusion Mode** (Recommended)
   - Light affects ONLY linked objects
   - Everything else is unaffected
   - More predictable

2. **Exclusion Mode**
   - Light affects ALL objects EXCEPT excluded ones
   - Use when most objects should be lit

---

### Creating Light Links

#### Method 1: Quick Link (Simple)

**Link selected lights to selected objects:**

1. **Select your objects** (e.g., your main product)
2. **Shift-click to add lights** to selection
3. Go to **"Light Linking"** section in panel
4. Click **"Link Selected Lights to Objects"**

✅ Now those lights only affect those objects!

---

#### Method 2: Collection Linking

**Link lights to entire collections:**

1. Ensure objects are in a collection
2. **Select lights**
3. Go to Light Linking section
4. **Choose collection** from dropdown
5. Click **"Link to Collection"**

✅ Lights affect all objects in that collection!

**💡 Pro Tip**: Use collections for organized workflows.

---

#### Method 3: Manual Linking Panel

**For precise control:**

1. Go to Light Linking section
2. Find **"Light-Object Relationships"** panel
3. Each light shows:
   - Light name
   - Linked/Excluded objects list
   - Add/Remove buttons
4. **Click "+"** to add object to light
5. **Click "-"** to remove object from light

---

### Step-by-Step Examples

#### Example 1: Product with Rim Light

**Goal**: Create a rim light that ONLY affects the product, not the background.

1. **Setup**: Product on pedestal with background plane
2. **Create rim light** behind product
3. **Select rim light only**
4. In Light Linking panel:
   - Click **"Add Object"**
   - Select your product from list
   - Click confirm
5. **Test**: Rim light now only lights the product!

**Result**: Clean rim lighting without affecting background.

---

#### Example 2: Multi-Object Scene

**Goal**: Each object has its own key light.

1. **Setup**: 3 products in scene (A, B, C)
2. **Create 3 key lights** (Light_A, Light_B, Light_C)
3. **Link Light_A** to Product A only
4. **Link Light_B** to Product B only
5. **Link Light_C** to Product C only
6. **Add fill lights** with no linking (affects all)

**Result**: Independent control over each product's lighting.

---

### Managing Light Links

#### View Current Links

1. Go to Light Linking section
2. Expand **"Current Links"** panel
3. See all light-object relationships
4. Format: "Light Name → Object Name"

#### Clear All Links for a Light

1. Select light
2. Click **"Clear All Links"** button
3. Light now affects all objects again (default)

#### Clear All Links in Scene

1. Go to Light Linking section
2. Click **"Clear All Scene Links"**
3. ⚠️ Confirmation required
4. All lights return to default (affect everything)

---

### Light Linking Best Practices

✅ **DO:**
- Use collections for large scenes
- Name lights clearly (RimLight_ProductA)
- Start simple: Link one light at a time
- Test renders frequently
- Document complex linking setups

❌ **DON'T:**
- Create overly complex linking (hard to manage)
- Forget to check render results
- Link lights to hidden objects (confusing)
- Mix linking modes randomly

**💡 Workflow Tip:**
1. Set up basic scene lighting (affects all)
2. Add fill/ambient (affects all)
3. Add accent/rim lights (linked to specific objects)
4. Fine-tune each light independently

---

### Troubleshooting Light Linking

**Problem**: Light doesn't affect anything
- **Solution**: Check if light has links - clear them to reset

**Problem**: Can't see linking effect
- **Solution**: Ensure viewport shading shows lighting (Solid/Material/Rendered)

**Problem**: Light affects wrong objects
- **Solution**: Clear links, start over with clearer naming

---
