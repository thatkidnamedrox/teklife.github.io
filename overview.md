# TEKLIFE Footwork Digital Musicology Analysis

## Overview
An interactive D3.js visualization dashboard exploring Teklife footwork music through the lens of digital musicology. Combines audio analysis features (extracted via Librosa) with YouTube metadata to reveal the sonic and cultural characteristics of this Chicago-based electronic music genre.

## Complete Visualization List

### 1. Tempo Distribution & BPM Clustering
**Insight**: Reveals the characteristic ~160 BPM tempo of footwork (often detected at half-time ~80 BPM)
- Histogram with gradient bars
- Reference lines for key BPM values (80 BPM half-time, 160 BPM classic footwork)
- Shows rhythmic DNA of the genre

### 2. Temporal Evolution
**Insight**: Tracks upload frequency and engagement from 2010-2025
- Dual-axis chart showing uploads and views
- Area chart for upload count
- Line chart for average views
- Reveals growth of Teklife on YouTube

### 3. Sonic Fingerprint (Spectral Characteristics)
**Insight**: Maps the sonic signature of footwork—bright, energetic, dynamic
- X-axis: Spectral centroid (brightness)
- Y-axis: RMS energy
- Size: Onset strength (rhythmic intensity)
- Color: Tempo clustering (cyan → green → pink gradient)
- **Interactive**: Click any point to open track on YouTube

### 4. Feature Correlation Matrix
**Insight**: Shows relationships between audio features
- Heatmap of correlations between 8 key features
- Color scale from cyan (negative) to pink (positive)
- Reveals which features move together
- Understanding what makes footwork distinctive

### 5. Artist Network & Output
**Insight**: Ecosystem of Teklife artists and channels
- Bubble size: Track count
- Color: Average engagement (cyan to pink)
- **Interactive**: Drag nodes to explore relationships
- Top 20 artists by output

### 6. Popularity vs. Sonic Innovation
**Insight**: Does experimentation correlate with engagement?
- X-axis: Spectral variance (sonic experimentation)
- Y-axis: View count (log scale)
- Trend line shows relationship
- **Interactive**: Click points to explore tracks

### 7. MFCC Timbre Space
**Insight**: Maps timbral characteristics using first two MFCCs
- X-axis: MFCC 1 (overall spectral shape)
- Y-axis: MFCC 2 (spectral detail)
- Size: View count
- Color: Tempo (viridis color scale)
- Reveals clusters of similar timbres

### 8. Harmonic Complexity
**Insight**: Chroma features reveal harmonic and tonal content
- X-axis: Chroma mean (harmonic content level)
- Y-axis: Chroma std (harmonic variation)
- Color: Spectral contrast (plasma color scale)
- Shows tracks with rich harmonic vs. percussive focus

### 9. Spectral Profile
**Insight**: Frequency distribution characteristics
- X-axis: Spectral bandwidth (frequency spread)
- Y-axis: Spectral rolloff (where most energy is concentrated)
- Size: RMS energy
- Color: Tempo (turbo color scale)
- Reveals the "shape" of each track's frequency content

### 10. Rhythmic Intensity Distribution
**Insight**: Histogram of onset strength across all tracks
- Shows distribution of rhythmic "punch"
- Gradient colored bars (cyan → green → pink)
- Reveals common intensity profiles in footwork
- Higher onset = more aggressive, punchy rhythms

### 11. Texture Analysis (Zero-Crossing Rate)
**Insight**: Percussive and noise content analysis
- X-axis: Zero-crossing rate (noisiness/percussive content)
- Y-axis: Spectral bandwidth
- Size: Onset strength
- Color: Energy level (cool color scale)
- High ZCR = more high-frequency, percussive elements

### 12. Multi-Dimensional Feature Space
**Insight**: Parallel coordinates showing all features simultaneously
- 7 dimensions: Tempo, Brightness, Energy, Onset, ZCR, Chroma, Contrast
- Each line = one track
- Color: Tempo (rainbow scale)
- Reveals patterns across multiple dimensions
- **Interactive**: Hover to highlight individual tracks

## Key Musicological Findings

### Tempo Characteristics
- Average BPM: ~107 (with peaks at ~80 and ~160)
- The half-time detection phenomenon is common
- True footwork tempo is typically 160 BPM

### Sonic Profile
- **Bright & Energetic**: High spectral centroids (2000-4000 Hz)
- **Dynamic Range**: Significant RMS energy variation
- **Rhythmic Complexity**: Strong onset strength values (1.0-2.5)
- **Spectral Contrast**: High variance indicating dense, layered productions
- **Timbral Diversity**: MFCC analysis shows wide range of timbres
- **Harmonic vs. Percussive**: Chroma analysis reveals mix of harmonic and percussive-focused tracks

### Textural Characteristics
- **High ZCR**: Indicates percussive, noisy elements typical of footwork
- **Wide Spectral Bandwidth**: Shows broad frequency content
- **Variable Spectral Rolloff**: Different "weights" in frequency distribution
- **Strong Onset Patterns**: Consistent rhythmic intensity

### Community Insights
- **TEKLIFE Records**: Dominant presence (124 tracks)
- **Upload Patterns**: Increased activity in recent years (2020-2025)
- **Engagement**: Wide variation in view counts (1k to 6.5k avg)
- **Innovation**: Weak correlation between spectral experimentation and popularity

## Color Schemes by Visualization

- **Tempo-based**: Cyan (#00d4ff) → Green (#00ff41) → Pink (#ff0080)
- **Correlation**: Cyan (#00d4ff) → Dark → Pink (#ff0080)
- **MFCC**: Viridis (purple → green → yellow)
- **Chroma**: Plasma (purple → pink → yellow)
- **Spectral Profile**: Turbo (blue → cyan → green → yellow → red)
- **ZCR**: Cool (cyan → purple)
- **Parallel Coordinates**: Rainbow (full spectrum)

## Technical Stack
- **D3.js v7**: Data visualization
- **Librosa**: Audio feature extraction (Python)
- **YouTube Data**: Metadata and engagement metrics
- **HTML/CSS/JS**: Frontend implementation
- **Color Scales**: d3-scale-chromatic interpolators

## Dataset
- **208 tracks** analyzed
- **Date Range**: 2010-2025
- **Audio Features**: 
  - Temporal: Tempo, beats, duration
  - Spectral: Centroid, rolloff, bandwidth, contrast
  - Timbral: MFCCs (5 coefficients)
  - Harmonic: Chroma features
  - Rhythmic: Onset strength, zero-crossing rate
  - Energy: RMS energy
- **Metadata**: Views, likes, upload dates, artists, channels

## Usage
1. Open `teklife-footwork-analysis.html` in a modern web browser
2. Ensure `yt_clean_analysis.json` and `yt_clean_metadata.json` are in the same directory
3. Wait for loading animation to complete
4. Interact with visualizations:
   - **Hover** for detailed information
   - **Click** data points to open tracks on YouTube
   - **Drag** artist nodes in the network visualization
   - **Explore** patterns across 12 different perspectives

## Performance
- Initial load: ~2-3 seconds
- Smooth animations with staggered delays
- Optimized rendering for 200+ data points per visualization
- Responsive to hover/click interactions

## Browser Compatibility
- Chrome/Edge: ✅ Full support
- Firefox: ✅ Full support
- Safari: ✅ Full support  
- Mobile: ✅ Responsive design

## File Structure
```
teklife-footwork-analysis.html (84KB, 2088 lines)
├── Header with title and subtitle
├── Stats cards (5 metrics)
├── 12 Visualization sections
├── Footer with credits
└── Interactive tooltip system
```

---

**Built for exploring the digital musicology of Teklife footwork**  

*Now with 12 visualizations covering tempo, spectral, timbral, harmonic, rhythmic, and textural features*

