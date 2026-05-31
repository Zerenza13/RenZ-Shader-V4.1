# Contributing to RenZ Shader V4.1

Thank you for your interest in contributing! Here's how you can help improve the shader.

## Ways to Contribute

### 1. Report Bugs 🐛
- Create an issue with clear description
- Include your device info (model, Android/Windows version)
- Describe the steps to reproduce
- Attach screenshots if possible

### 2. Suggest Improvements 💡
- Post feature requests in Discussions
- Explain the visual enhancement you want
- Reference similar shaders if applicable
- Provide performance impact estimate

### 3. Code Contributions 📝
- Fork the repository
- Create a feature branch
- Make your changes
- Test thoroughly
- Submit a pull request

### 4. Content Contributions 🎨
- Create particle textures
- Design shader themes/variants
- Write tutorials
- Create comparison videos

## Development Guidelines

### Shader Code Standards
```glsl
// DO:
✅ Use meaningful variable names
✅ Add comments for complex calculations
✅ Optimize for mobile first
✅ Test on low-end devices
✅ Follow GLSL ES 1.00 syntax

// DON'T:
❌ Use features beyond OpenGL ES 3.0
❌ Create overly complex shaders
❌ Ignore performance impact
❌ Break existing functionality
❌ Use hard-coded magic numbers without explanation
```

### Performance Requirements
- Low-end device: Maintain 20+ FPS
- Mid-range device: Maintain 40+ FPS
- High-end device: 50+ FPS target

### Testing Checklist
- [ ] Tested on Android device
- [ ] Tested on Windows Bedrock
- [ ] Performance profiled
- [ ] No visual glitches
- [ ] Documentation updated
- [ ] No breaking changes

## Pull Request Process

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/AmazingFeature`)
3. **Commit** your changes (`git commit -m 'Add: AmazingFeature'`)
4. **Push** to the branch (`git push origin feature/AmazingFeature`)
5. **Open** a Pull Request
6. **Wait** for review and feedback
7. **Update** based on review comments
8. **Merge** when approved

### PR Title Format
```
[Type]: Brief description

Types: Add, Fix, Improve, Optimize, Refactor, Docs
```

Examples:
- `Add: Water reflection enhancement`
- `Fix: Aurora color artifacts on low-end devices`
- `Improve: Cloud rendering performance`
- `Optimize: Particle shader memory usage`

## Code Review Process

### What We Look For:
- ✅ Code quality and readability
- ✅ Performance impact
- ✅ Compatibility (all devices/versions)
- ✅ Documentation updates
- ✅ Testing evidence

### Feedback Timeline:
- Initial review: 1-3 days
- Revision period: 1 week
- Final approval: 1-2 days

## Issue Templates

### Bug Report
```markdown
**Device Info:**
- Model: [e.g., Xiaomi Redmi Note 7]
- OS: [Android X.X or Windows 10/11]
- GPU: [if known]

**Expected Behavior:**
[Describe what should happen]

**Actual Behavior:**
[Describe what happens instead]

**Steps to Reproduce:**
1. Open Minecraft
2. Apply shader
3. [...]

**Screenshots:**
[Attach images]
```

### Feature Request
```markdown
**Description:**
[Clear description of the feature]

**Use Case:**
[Why you need this]

**Performance Impact:**
[Estimated FPS impact]

**Similar to:**
[Other shaders that do this]
```

## Commit Message Format

```
[Type]: Description

[Optional detailed explanation]

- Bullet points for multiple changes
- One change per line
```

Examples:
```
Add: Aurora effect with wave animation

- Implemented green, purple, cyan aurora colors
- Added sine wave animation
- Nightness-based intensity control

Fix: Water shader transparency issue

- Changed alpha blending mode
- Adjusted depth calculation
- Tested on low-end devices
```

## Branch Naming

```
feature/    - New features
fix/        - Bug fixes
improve/    - Improvements
optimize/   - Performance optimization
docs/       - Documentation
refactor/   - Code refactoring
```

Examples:
- `feature/enhanced-water`
- `fix/aurora-flickering`
- `optimize/particle-system`

## Style Guide

### File Naming
```
- shader files: lowercase with extension (.vertex, .fragment)
- documentation: PascalCase with extension (.md)
- config files: lowercase with extension (.json, .material)
```

### Code Comments
```glsl
// For single line
// This calculates the wave height

// For multi-line
/*
 * Complex calculation:
 * - First part explanation
 * - Second part explanation
 * - Result interpretation
 */

// For important notes
// TODO: Optimize this calculation for mobile
// HACK: Temporary fix for aurora flicker
// BUG: Water transparency breaks on old GPUs
```

## Documentation Standards

### README Updates
- Keep it concise but comprehensive
- Add table of contents for long docs
- Use clear headings and formatting
- Include examples where applicable

### Code Documentation
- Document all uniform variables
- Explain complex algorithms
- Note performance considerations
- Link to related shaders/techniques

## Communication

### Discussion Channels
- **GitHub Issues:** Bug reports & bug fixes
- **GitHub Discussions:** Feature ideas & general questions
- **Pull Requests:** Code review & implementation

### Be Respectful
- Assume good intentions
- Provide constructive feedback
- Help newer contributors
- Welcome diverse perspectives

## Recognition

Contributors will be acknowledged in:
- README.md contributors section
- Release notes for major contributions
- GitHub contributors page

## Questions?

- Read existing issues/PRs first
- Check documentation thoroughly
- Ask in Discussions before opening issues
- Comment on related issues if uncertain

---

**Thank you for making RenZ Shader V4.1 better!** 🚀

**Happy coding!** 🎨✨
