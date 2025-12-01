# Quick Reference Guide - TEKLIFE Footwork Analysis

## What Each Visualization Tells You

### 🎵 Basic Characteristics

**1. Tempo Distribution**
- Look for: Two main peaks (around 80 BPM and 160 BPM)
- Meaning: Most footwork detected at half-time; actual tempo is ~160 BPM
- Footwork signature: Fast, syncopated rhythms

**2. Temporal Evolution**  
- Look for: Upload frequency spikes, view trends
- Meaning: Genre's growth on YouTube over time
- Pattern: Increased activity 2020-2025

### 🔊 Sonic Identity

**3. Sonic Fingerprint (Centroid vs Energy)**
- X-axis: Spectral Centroid = Brightness (2000-4000 Hz = bright)
- Y-axis: RMS Energy = Loudness (higher = more powerful)
- Circle size: Onset Strength = Rhythmic punch
- Color: Tempo (cyan = slow, pink = fast)
- Footwork cluster: Upper-right quadrant (bright + energetic)

**4. MFCC Timbre Space**
- Maps: Overall "texture" and "tone color" of tracks
- Clusters: Similar-sounding tracks group together
- Size: Popularity (bigger = more views)
- Footwork signature: Wide spread indicates timbral diversity

**5. Spectral Profile (Bandwidth vs Rolloff)**
- X-axis: Bandwidth = How "wide" the frequency spectrum is
- Y-axis: Rolloff = Where most energy concentrates (Hz)
- High rolloff: More high-frequency content
- Wide bandwidth: More complex frequency distribution

### 🎹 Musical Content

**6. Harmonic Complexity (Chroma)**
- X-axis: Chroma Mean = Amount of pitched/harmonic content
- Y-axis: Chroma Std = How much harmony changes
- Low chroma: Percussive-focused tracks
- High chroma + high std: Melodic, dynamic tracks
- Footwork tends toward: Lower-left (percussion-focused)

**7. Rhythmic Intensity**
- Histogram of "rhythmic punch" across all tracks
- Higher values = More aggressive, hard-hitting beats
- Peak around 1.0-1.5 = Footwork's characteristic intensity
- Outliers (2.5+) = Exceptionally punchy productions

**8. Texture Analysis (ZCR)**
- X-axis: Zero-Crossing Rate = Noisiness/percussion
- Y-axis: Bandwidth = Frequency spread
- High ZCR = More hi-hats, snares, noisy elements
- Footwork signature: Higher ZCR than most electronic music

### 📊 Relationships & Patterns

**9. Feature Correlation Matrix**
- Red/Pink cells = Features move together (positive correlation)
- Blue/Cyan cells = Features move opposite (negative correlation)
- Dark cells = No relationship
- Key insight: Which features define footwork's sound

**10. Innovation vs Popularity**
- X-axis: Spectral Variance = Sonic experimentation
- Y-axis: Views = Popularity
- Trend line: Does experimentation = more views?
- Finding: Weak correlation (experimentation ≠ guaranteed popularity)

**11. Multi-Dimensional Space (Parallel Coordinates)**
- Each line = One track across 7 dimensions
- Crossing patterns = Feature relationships
- Color = Tempo (rainbow spectrum)
- Divergent lines = Outlier tracks
- Parallel lines = Similar production approach

### 👥 Community & Culture

**12. Artist Network**
- Bubble size = Number of tracks produced
- Color = Average engagement (cyan = low views, pink = high views)
- TEKLIFE Records: Largest bubble (dominant producer)
- Drag bubbles to explore relationships

## Reading the Colors

### Tempo-Based (Most Common)
- **Cyan** (#00d4ff) = ~75-100 BPM (slow/half-time)
- **Green** (#00ff41) = ~120-140 BPM (mid-range)
- **Pink** (#ff0080) = ~160+ BPM (fast/true footwork)

### Energy-Based
- **Cool colors** (blue/cyan) = Low energy
- **Warm colors** (yellow/red) = High energy

### Correlation-Based
- **Cyan** = Negative correlation
- **Dark** = No correlation
- **Pink** = Positive correlation

## Key Metrics Explained

### Spectral Features
- **Centroid**: "Brightness" - higher Hz = brighter sound
- **Rolloff**: Where 85% of energy sits in spectrum
- **Bandwidth**: Width of frequency distribution
- **Contrast**: Difference between peaks and valleys

### Timbral Features
- **MFCC 1-5**: Capture overall sound texture/tone
- **ZCR**: Zero-crossing rate = noisiness/percussion

### Harmonic Features
- **Chroma Mean**: Amount of pitched content
- **Chroma Std**: How much harmony changes

### Rhythmic Features
- **Onset Strength**: How "punchy" the beats are
- **Tempo**: Detected BPM (often half-time)
- **RMS Energy**: Overall loudness/power

## Interaction Guide

### Mouse Actions
- **Hover**: See detailed info in tooltip
- **Click**: Open track on YouTube (scatter plots)
- **Drag**: Move artist bubbles (network viz)

### What to Look For

**Outliers** = Unusual tracks that break patterns
**Clusters** = Groups of similar tracks
**Trends** = Lines/gradients showing relationships
**Density** = Where most tracks concentrate

## Footwork's Sonic Signature

Based on all visualizations:

✅ **Tempo**: ~160 BPM (detected as 80 BPM half-time)
✅ **Brightness**: High spectral centroid (2500-3500 Hz)
✅ **Energy**: Strong RMS (0.15-0.30)
✅ **Rhythm**: High onset strength (1.0-2.0)
✅ **Texture**: High zero-crossing rate (percussive)
✅ **Harmony**: Lower chroma (percussion-focused)
✅ **Timbre**: Diverse MFCC patterns
✅ **Intensity**: Aggressive, punchy sound

## Tips for Analysis

1. **Start with Tempo Distribution** - Understand the BPM landscape
2. **Check Sonic Fingerprint** - See where tracks cluster sonically
3. **Explore MFCC Space** - Find timbral similarities
4. **Examine Correlations** - Understand feature relationships
5. **Use Parallel Coordinates** - Compare across all dimensions
6. **Click tracks** - Listen to outliers and clusters on YouTube

## Common Patterns

- Most tracks cluster in "bright + energetic" region
- Tempo detection shows half-time phenomenon
- High ZCR indicates aggressive percussion
- Lower chroma = percussion-focused production
- TEKLIFE Records dominates artist ecosystem
- Innovation doesn't guarantee popularity
- Increased upload activity in recent years

---

**Use this guide while exploring the interactive dashboard to understand what each visualization reveals about Teklife footwork music!**
