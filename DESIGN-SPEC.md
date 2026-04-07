# PhD Thesis Visualization — Design Specification

## 논문 제목 (Working)
"Toxicity assessment of phthalate plasticizer mixtures in zebrafish at environmentally relevant concentrations based on global children's biomonitoring data"

## 정보 구조 (Information Architecture)

### Flow: Left → Right, 3단계 + 하단 3-Chapter 분기

```
STAGE 1              STAGE 2              STAGE 3
[Global BM Data] → [Dose Translation] → [Mixture Design] 
  4 countries         PBK Modeling          Full(7) vs Reduced(5)
  Children urine      Human→Fish            ToxPiR selection
                      Plasma conc.
                                    ↓
                         ┌─────────┼─────────┐
                      Ch.1        Ch.2       Ch.3
                    Develop.    Metab/Inf.  Chronic+Recovery
                    (Embryo)    (Adult)     (Subchronic)
```

## 각 요소 상세

### Stage 1: Global Biomonitoring
- 4 국가 아이콘: 🇰🇷 Korea, 🇹🇭 Thailand, 🇧🇩 Bangladesh, 🇪🇬 Egypt
- "Children's urine samples" 표기
- Detection Frequency >70% 기준 명시

### Stage 2: PBK Modeling (Dose Translation)
- Human silhouette → Arrow → Fish silhouette
- "Reverse dosimetry" or "PBK modeling"
- Urine concentration → Fish plasma concentration

### Stage 3: Mixture Design
- Full Mixture: 7 compounds (DMP, DEP, DiBP, DnBP, DEHP, DiNP, DEHTP)
- ToxPiR → identify Top 2 Risk Drivers (country-specific)
- Reduced Mixture: 5 compounds (minus top 2 drivers)
- Visual: 7 circles → remove 2 highlighted → 5 circles

### Chapter 1: Developmental Toxicity
- Model: Zebrafish embryo/larvae icon
- Endpoints: Thyroid disruption, Image-based phenotyping, Behavioral changes
- Compare: Full vs Reduced

### Chapter 2: Metabolic/Inflammatory Toxicity  
- Model: Adult zebrafish icon
- Endpoints: Oxidative stress (ROS), Lipid metabolism, Inflammation
- Compare: Full vs Reduced

### Chapter 3: Chronic Exposure + Recovery
- Timeline: 30-day exposure → 60-day recovery (clean water)
- At 30d: Thyroid hormones + Transcriptomics
- At 60d (male): Sperm quality + Testosterone
- Key question: "Are effects reversible?"

## Design System

### Color Palette (Nature-inspired, muted scientific)
- Primary: #2D7D9A (teal/petrol blue) — main flow, headers
- Secondary: #E8734A (warm coral) — highlights, risk drivers
- Tertiary: #6B8E6B (sage green) — Chapter 3 recovery
- Neutral: #4A4A4A (dark gray text), #F5F5F0 (warm white bg)
- Light accents: #E8E4DF (warm gray for cards)

### Typography
- Headers: Inter Bold or Helvetica Neue Bold, 14-16pt
- Body: Inter Regular, 10-11pt
- Labels: Inter Light, 8-9pt
- All caps for stage labels only

### Layout
- Total size: 1200 x 700px (landscape, 16:9-ish for presentation)
- Also exportable as A4 landscape for print
- Grid: 12-column with generous whitespace
- Margins: 40px all sides

### Visual Elements
- Minimal line icons (not emoji) for organisms
- Rounded rectangles for content blocks (radius: 8px)
- Thin connecting lines (1.5px) with small arrowheads
- No drop shadows, no gradients — flat design
- Subtle dotted borders for "comparison" blocks

### Key Design Principles
1. LESS IS MORE — only essential text
2. Visual hierarchy through size, not decoration
3. Color = meaning (teal=flow, coral=highlight, green=recovery)
4. White space is a feature, not waste
5. Every element must earn its place
