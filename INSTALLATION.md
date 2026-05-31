# RenZ Shader V4.1 - Installation Guide

## Quick Start Guide

### 🎮 For Minecraft PE on Android

#### Method 1: Direct File Installation
1. **Download** the shader pack (RenZ-Shader-V4.1.zip)
2. **Move** the zip file to your Downloads or Documents folder
3. **Open** Minecraft PE
4. Go to **Settings** → **Global Resources**
5. Click **Browse** and locate the zip file
6. **Select** and apply the shader
7. Restart Minecraft PE

#### Method 2: Manual Installation
1. Extract the shader zip file
2. Connect phone to PC via USB or use file manager
3. Navigate to: `Android/data/com.mojang.minecraftpe/files/resource_packs/`
4. Paste the extracted folder there
5. Open Minecraft PE and apply from Settings

#### Method 3: Using File Manager App
1. Download shader pack to Downloads folder
2. Open file manager app
3. Go to: `Android → data → com.mojang.minecraftpe → files → resource_packs`
4. Extract zip file here
5. Open Minecraft PE, go to Settings → Global Resources → Apply

### 💻 For Windows (Bedrock Edition)

#### Step 1: Locate Resource Packs Folder
1. Press **Win + R**
2. Type: `%LOCALAPPDATA%`
3. Navigate: `Packages → Microsoft.MinecraftUWP_8wekyb3d8bbwe → LocalState → games → com.mojang → resource_packs`
4. Open **resource_packs** folder

#### Step 2: Add Shader Pack
1. Extract **RenZ-Shader-V4.1.zip** to this folder
2. Folder name should be: **RenZ-Shader-V4.1**

#### Step 3: Apply in Minecraft
1. Open **Minecraft Bedrock Edition**
2. Click **Settings** (gear icon)
3. Go to **Global Resources**
4. Find **RenZ Shader V4.1** in the list
5. Click it and select **Apply**
6. Restart Minecraft

### 📱 Device Requirements

**Minimum:**
- Android 6.0 (API 23) or higher
- 2GB RAM (minimum)
- OpenGL ES 3.0 or higher
- 100MB free storage

**Recommended:**
- Android 9.0 (API 28) or higher
- 4GB+ RAM
- OpenGL ES 3.1 or higher
- 200MB+ free storage

**Windows:**
- Windows 10 Build 14393 or newer
- 4GB+ RAM
- GPU with DirectX 12 support

## Troubleshooting

### Issue: Shader pack not appearing in list

**Solution:**
1. Ensure zip file is in correct folder
2. Check file name matches exactly: `RenZ-Shader-V4.1`
3. Try re-extracting the zip file
4. Clear Minecraft cache:
   - Android: Settings → Apps → Minecraft PE → Storage → Clear Cache
   - Windows: Settings → App → Minecraft → Reset

### Issue: Shader not applying / game crashes

**Solution:**
1. **Verify MCPE version:** Must be 1.21+
2. **Check OpenGL version:**
   - Settings → Video → Advanced Graphics → Renderer
   - Should be OpenGL ES 3.0+
3. **Disable other resource packs:**
   - Disable all other packs temporarily
   - Apply only RenZ Shader
4. **Try default settings:**
   - Delete any custom configs
   - Use default shader settings

### Issue: Low FPS / Performance lag

**Solution 1 - Reduce Graphics:**
1. Settings → Video
2. Set Render Distance: 8-12 chunks (instead of 16+)
3. Disable Animated Textures
4. Lower resolution if available

**Solution 2 - Device Optimization:**
1. Close background apps
2. Restart Minecraft
3. Clear game cache
4. Update GPU drivers (if on Windows)

**Solution 3 - Shader Adjustments:**
1. Disable Aurora effects
2. Reduce particle density
3. Lower water quality temporarily

### Issue: Visual glitches (white lines, missing textures)

**Solution:**
1. Verify all files extracted properly
2. Check file permissions (Android)
3. Reinstall shader pack
4. Try on different world

### Issue: "Cannot load shader" error

**Solution:**
1. Update Minecraft to latest version
2. Check file path is correct
3. Ensure folder name matches exactly
4. Try extracting zip in a different way
5. Verify GPU supports OpenGL ES 3.0+

### Issue: Water looks weird / too bright

**Solution:**
1. This might be normal on some devices
2. Try adjusting brightness in Minecraft settings
3. Update GPU drivers
4. Try disabling water reflections in config (if available)

## Performance Optimization

### For Low-End Devices (1-2GB RAM):
```
Render Distance: 8 chunks
Particle Distance: 16 blocks
Max Entities: 50
Animated Textures: OFF
Fancy Graphics: OFF
```

### For Mid-Range Devices (4GB RAM):
```
Render Distance: 12 chunks
Particle Distance: 32 blocks
Max Entities: 100
Animated Textures: ON
Fancy Graphics: ON
```

### For High-End Devices (6GB+ RAM):
```
Render Distance: 16+ chunks
Particle Distance: 64 blocks
Max Entities: 200+
All Effects: Maximum
```

## Advanced Configuration

### Editing Shader Settings (Optional)

If you want to fine-tune the shader:

1. Navigate to shader folder
2. Open `shaders/glsl/renderchunk.fragment`
3. Modify constants:
   ```glsl
   // Adjust these values:
   const vec3 SUN_COLOR = vec3(1.0, 0.7, 0.2);      // Sun color
   const vec3 AMBIENT_COLOR = vec3(0.5, 0.6, 0.8);  // Sky color
   ```
4. Save and restart Minecraft

**Common Adjustments:**
- Increase brightness: Multiply AMBIENT_COLOR by 1.2
- Reduce bloom: Divide specular by 2
- More saturated colors: Multiply colors by 1.1-1.3

## Uninstalling

### Android:
1. Open Minecraft PE
2. Settings → Global Resources
3. Find RenZ Shader V4.1
4. Click and select "Delete"
5. Or manually delete from: `Android/data/com.mojang.minecraftpe/files/resource_packs/`

### Windows:
1. Navigate to resource_packs folder
2. Delete **RenZ-Shader-V4.1** folder
3. Restart Minecraft

## Getting Help

If you encounter issues not covered here:

1. **Check logs:** Look for error messages in Minecraft output
2. **Verify files:** Ensure all files are present and uncorrupted
3. **Try clean install:** Delete and reinstall shader pack
4. **Update drivers:** Keep GPU and system drivers updated
5. **Contact support:** Report issue with device info and logs

---

**Happy shading!** 🎨✨
