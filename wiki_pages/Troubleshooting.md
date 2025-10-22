## Troubleshooting

### Common Issues

#### "HDRI Grid Shows No HDRIs"

**Problem**: Grid popup is empty.

**Solutions:**
1. Check HDRI Assets Folder path in preferences
2. Ensure folder contains `.hdr` or `.exr` files
3. Try restarting Blender
4. Check file permissions on HDRI folder

---

#### "Scenario Switching Doesn't Work"

**Problem**: Clicking scenario doesn't change lights.

**Solutions:**
1. Ensure lights were saved in scenario (Update Scenario)
2. Check if lights are hidden in Outliner
3. Exit any active blend modes
4. Try recreating scenario from scratch

---

#### "Fast Light Edit Mode Won't Start"

**Problem**: Edit mode button does nothing.

**Solutions:**
1. Check "Light Edit Enabled" in preferences
2. Ensure light is selected
3. Check if light type is supported (Area/Point/Spot/Sun)
4. Restart Blender if issue persists

---

#### "Batch Operations Affect Nothing"

**Problem**: Batch operation runs but nothing changes.

**Solutions:**
1. Ensure lights are selected first
2. Check if lights are in locked collection
3. Verify operation parameters are correct
4. Use Outliner to verify selection

---

#### "Light Linking Not Visible in Viewport"

**Problem**: Can't see linking effect in 3D View.

**Solutions:**
1. Switch to Material Preview or Rendered viewport shading
2. Solid shading doesn't show all lighting effects
3. Ensure lights are enabled in viewport
4. Check render engine settings (EEVEE vs Cycles)

---

### Performance Issues

#### "Scene is Slow with Many Scenarios"

**Solutions:**
1. Reduce number of scenarios (keep under 20)
2. Use scenario blending instead of many variations
3. Delete unused scenarios
4. Simplify scene (fewer lights per scenario)

#### "HDRI Grid is Slow to Load"

**Solutions:**
1. Reduce HDRI count in folder (keep under 50)
2. Use smaller HDRI resolution for previews
3. Store HDRIs on SSD instead of HDD
4. Close other applications

---

### Getting Help

**Still having issues?**

1. **Check README.md** for basic info
2. **Review this documentation** for detailed steps
3. **Contact Support:**
   - Email: [YOUR EMAIL]
   - Discord: [YOUR DISCORD]
   - Purchase platform support
4. **Include in support request:**
   - Blender version
   - Light Manager Pro version
   - Description of issue
   - Steps to reproduce
   - Screenshots if relevant

---
