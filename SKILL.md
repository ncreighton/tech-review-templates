# Tech Review Templates

Comprehensive review page templates and component library for tech review sites. Creates conversion-optimized, trust-building review content.

## Sites Using This Skill

| Site | Focus | Primary Components |
|------|-------|-------------------|
| pulsegearreviews.com | Fitness tech | Workout metrics, battery tests, comfort ratings |
| wearablegearreviews.com | Wearables | Health accuracy, data charts, sensor comparisons |
| smarthomegearreviews.com | Smart home | Ecosystem compatibility, setup ease, integration |

---

## Review Article Types

### Type 1: Single Product Deep Review
**URL pattern:** `/product-name-review/`
**Word count:** 2,500-4,000 words

**Sections:**
1. Quick Verdict Box (above fold)
2. Who Should Buy / Who Should Skip
3. Design & Build Quality
4. Key Features Deep Dive
5. Performance Testing
6. Battery/Power
7. Companion App Experience
8. Competition Comparison
9. Final Verdict & Rating
10. FAQ Section

### Type 2: Best Of Roundup
**URL pattern:** `/best-category-year/`
**Word count:** 3,000-5,000 words

**Sections:**
1. Quick Picks Summary Table
2. How We Tested
3. What to Look For (Buyer's Guide)
4. Individual Product Reviews (500 words each)
5. Comparison Table
6. FAQ Section
7. Methodology

### Type 3: Versus Comparison
**URL pattern:** `/product-a-vs-product-b/`
**Word count:** 2,000-3,000 words

**Sections:**
1. Quick Verdict (Winner Declared)
2. Side-by-Side Specs Table
3. Design Comparison
4. Feature-by-Feature Breakdown
5. Performance Head-to-Head
6. Price & Value Analysis
7. Who Should Buy Which
8. FAQ

---

## Page Templates by Site

### PulseGearReviews.com (Fitness Tech)

**Quick Verdict Component:**
```html
<div class="quick-verdict fitness-style">
  <div class="verdict-header">
    <div class="product-visual">
      <img src="product.jpg" alt="Fitness Tracker" />
      <span class="badge-rating">9.2</span>
    </div>
    <div class="verdict-content">
      <h2 class="product-name">Garmin Forerunner 965</h2>
      <div class="verdict-tags">
        <span class="tag tag-best">Best for Runners</span>
        <span class="tag tag-premium">Premium Pick</span>
      </div>
      <p class="verdict-summary">
        The most complete running watch we've tested, with exceptional GPS accuracy 
        and training features that justify the premium price.
      </p>
      <div class="verdict-highlights">
        <div class="highlight">
          <span class="highlight-icon">🔋</span>
          <span class="highlight-text">23-day battery</span>
        </div>
        <div class="highlight">
          <span class="highlight-icon">🎯</span>
          <span class="highlight-text">Multi-band GPS</span>
        </div>
        <div class="highlight">
          <span class="highlight-icon">💪</span>
          <span class="highlight-text">Training load</span>
        </div>
      </div>
    </div>
  </div>
  <div class="verdict-footer">
    <div class="price-section">
      <span class="price-current">$599</span>
      <span class="price-source">Amazon</span>
    </div>
    <a href="#" class="btn-check-price">Check Current Price →</a>
  </div>
</div>
```

**Fitness Metrics Component:**
```html
<div class="fitness-metrics-card">
  <h4>Activity Tracking Accuracy</h4>
  <div class="metrics-grid">
    <div class="metric">
      <span class="metric-label">Step Count</span>
      <div class="accuracy-bar">
        <div class="accuracy-fill" style="width: 97%"></div>
      </div>
      <span class="metric-value">97% accurate</span>
    </div>
    <div class="metric">
      <span class="metric-label">Heart Rate</span>
      <div class="accuracy-bar">
        <div class="accuracy-fill" style="width: 94%"></div>
      </div>
      <span class="metric-value">94% vs chest strap</span>
    </div>
    <div class="metric">
      <span class="metric-label">GPS Distance</span>
      <div class="accuracy-bar">
        <div class="accuracy-fill" style="width: 99%"></div>
      </div>
      <span class="metric-value">99% accurate</span>
    </div>
    <div class="metric">
      <span class="metric-label">Sleep Tracking</span>
      <div class="accuracy-bar">
        <div class="accuracy-fill" style="width: 85%"></div>
      </div>
      <span class="metric-value">85% vs polysomnography</span>
    </div>
  </div>
  <p class="metrics-note">Tested over 30 days against reference devices</p>
</div>
```

**CSS for PulseGear:**
```css
/* Energy red accent throughout */
.fitness-style {
  --review-accent: #FF4136;
  --review-accent-light: #FF6B63;
  --review-badge-bg: #FF4136;
}

.fitness-metrics-card {
  background: var(--color-surface);
  border-radius: var(--radius-lg);
  padding: 1.5rem;
  border-left: 4px solid var(--review-accent);
}

.accuracy-bar {
  background: var(--color-border);
  height: 8px;
  border-radius: 4px;
  overflow: hidden;
}

.accuracy-fill {
  height: 100%;
  background: linear-gradient(90deg, var(--review-accent), var(--review-accent-light));
  border-radius: 4px;
}
```

---

### WearableGearReviews.com (Health Wearables)

**Health Data Visualization Component:**
```html
<div class="health-data-card">
  <h4>Health Sensor Accuracy Tests</h4>
  <div class="data-viz-wrapper">
    <div class="sensor-test">
      <div class="sensor-icon">❤️</div>
      <div class="sensor-info">
        <span class="sensor-name">Optical Heart Rate</span>
        <span class="sensor-rating excellent">Excellent</span>
      </div>
      <div class="sensor-detail">
        <span class="vs-reference">vs. Polar H10 chest strap</span>
        <span class="correlation">R² = 0.96</span>
      </div>
    </div>
    <div class="sensor-test">
      <div class="sensor-icon">🩸</div>
      <div class="sensor-info">
        <span class="sensor-name">SpO2 Sensor</span>
        <span class="sensor-rating good">Good</span>
      </div>
      <div class="sensor-detail">
        <span class="vs-reference">vs. Medical pulse oximeter</span>
        <span class="correlation">±2% deviation</span>
      </div>
    </div>
    <div class="sensor-test">
      <div class="sensor-icon">😴</div>
      <div class="sensor-info">
        <span class="sensor-name">Sleep Stages</span>
        <span class="sensor-rating good">Good</span>
      </div>
      <div class="sensor-detail">
        <span class="vs-reference">vs. Oura Ring Gen 3</span>
        <span class="correlation">82% agreement</span>
      </div>
    </div>
  </div>
</div>
```

**Battery Endurance Chart:**
```html
<div class="battery-chart-card">
  <h4>Real-World Battery Test</h4>
  <div class="battery-scenarios">
    <div class="scenario">
      <span class="scenario-name">Always-on Display + GPS</span>
      <div class="battery-bar-wrapper">
        <div class="battery-bar" style="width: 25%">
          <span class="battery-days">2 days</span>
        </div>
      </div>
    </div>
    <div class="scenario">
      <span class="scenario-name">Standard Use (AOD off)</span>
      <div class="battery-bar-wrapper">
        <div class="battery-bar" style="width: 50%">
          <span class="battery-days">4 days</span>
        </div>
      </div>
    </div>
    <div class="scenario">
      <span class="scenario-name">Battery Saver Mode</span>
      <div class="battery-bar-wrapper">
        <div class="battery-bar" style="width: 87%">
          <span class="battery-days">7 days</span>
        </div>
      </div>
    </div>
  </div>
  <p class="test-methodology">Tested with default settings, notifications enabled, 
     30 min daily workout tracking.</p>
</div>
```

**CSS for WearableGear:**
```css
/* Health teal accent */
.health-style {
  --review-accent: #1ABC9C;
  --review-accent-light: #48D1B5;
  --review-badge-bg: #1ABC9C;
}

.sensor-rating {
  padding: 0.25rem 0.75rem;
  border-radius: var(--radius-full);
  font-size: 0.75rem;
  font-weight: 600;
  text-transform: uppercase;
}

.sensor-rating.excellent {
  background: #22C55E20;
  color: #22C55E;
}

.sensor-rating.good {
  background: #1ABC9C20;
  color: #1ABC9C;
}

.sensor-rating.average {
  background: #F59E0B20;
  color: #F59E0B;
}

.correlation {
  font-family: var(--font-mono);
  font-size: 0.875rem;
  color: var(--color-text-muted);
}
```

---

### SmartHomeGearReviews.com (Smart Home)

**Ecosystem Compatibility Matrix:**
```html
<div class="compatibility-matrix">
  <h4>Smart Home Ecosystem Compatibility</h4>
  <table class="compat-table">
    <thead>
      <tr>
        <th>Platform</th>
        <th>Status</th>
        <th>Features</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>
          <span class="platform-icon alexa"></span>
          Amazon Alexa
        </td>
        <td><span class="compat-badge full">Full Support</span></td>
        <td>Voice control, routines, groups</td>
      </tr>
      <tr>
        <td>
          <span class="platform-icon google"></span>
          Google Home
        </td>
        <td><span class="compat-badge full">Full Support</span></td>
        <td>Voice control, routines, rooms</td>
      </tr>
      <tr>
        <td>
          <span class="platform-icon homekit"></span>
          Apple HomeKit
        </td>
        <td><span class="compat-badge partial">Via Matter</span></td>
        <td>Basic control, no automations</td>
      </tr>
      <tr>
        <td>
          <span class="platform-icon matter"></span>
          Matter
        </td>
        <td><span class="compat-badge full">Certified</span></td>
        <td>Cross-platform, local control</td>
      </tr>
    </tbody>
  </table>
</div>
```

**Setup Difficulty Rating:**
```html
<div class="setup-rating-card">
  <h4>Setup Experience</h4>
  <div class="setup-steps">
    <div class="step">
      <span class="step-number">1</span>
      <span class="step-name">Unboxing to Power</span>
      <span class="step-time">2 min</span>
    </div>
    <div class="step">
      <span class="step-number">2</span>
      <span class="step-name">App Connection</span>
      <span class="step-time">5 min</span>
    </div>
    <div class="step">
      <span class="step-number">3</span>
      <span class="step-name">Voice Assistant Link</span>
      <span class="step-time">3 min</span>
    </div>
  </div>
  <div class="setup-summary">
    <div class="total-time">
      <span class="time-label">Total Setup Time</span>
      <span class="time-value">~10 minutes</span>
    </div>
    <div class="difficulty-meter">
      <span class="difficulty-label">Difficulty</span>
      <div class="difficulty-dots">
        <span class="dot filled"></span>
        <span class="dot filled"></span>
        <span class="dot"></span>
        <span class="dot"></span>
        <span class="dot"></span>
      </div>
      <span class="difficulty-text">Easy</span>
    </div>
  </div>
</div>
```

**CSS for SmartHome:**
```css
/* Trust blue accent */
.smarthome-style {
  --review-accent: #0066CC;
  --review-accent-light: #3399FF;
  --review-badge-bg: #0066CC;
}

.compat-badge {
  padding: 0.25rem 0.75rem;
  border-radius: var(--radius-full);
  font-size: 0.75rem;
  font-weight: 600;
}

.compat-badge.full {
  background: #22C55E20;
  color: #22C55E;
}

.compat-badge.partial {
  background: #F59E0B20;
  color: #F59E0B;
}

.compat-badge.none {
  background: #EF444420;
  color: #EF4444;
}

.platform-icon {
  display: inline-block;
  width: 24px;
  height: 24px;
  margin-right: 0.5rem;
  vertical-align: middle;
}

.platform-icon.alexa { background: url('alexa.svg') no-repeat center; }
.platform-icon.google { background: url('google-home.svg') no-repeat center; }
.platform-icon.homekit { background: url('homekit.svg') no-repeat center; }
.platform-icon.matter { background: url('matter.svg') no-repeat center; }
```

---

## Universal Components

### Specs Table (All Sites)
```html
<div class="specs-table-wrapper">
  <h4>Technical Specifications</h4>
  <table class="specs-table">
    <tbody>
      <tr>
        <th>Display</th>
        <td>1.4" AMOLED, 454x454, Always-on</td>
      </tr>
      <tr>
        <th>Processor</th>
        <td>Qualcomm Snapdragon W5+ Gen 1</td>
      </tr>
      <tr>
        <th>Storage</th>
        <td>32GB internal</td>
      </tr>
      <tr>
        <th>Battery</th>
        <td>590mAh, up to 80 hours</td>
      </tr>
      <tr>
        <th>Water Resistance</th>
        <td>5ATM + IP68</td>
      </tr>
      <tr>
        <th>Connectivity</th>
        <td>Bluetooth 5.3, Wi-Fi, NFC, GPS</td>
      </tr>
      <tr>
        <th>Dimensions</th>
        <td>47 x 47 x 12.9mm</td>
      </tr>
      <tr>
        <th>Weight</th>
        <td>52g (without band)</td>
      </tr>
    </tbody>
  </table>
</div>
```

### Who Should Buy Box
```html
<div class="who-should-buy">
  <div class="should-buy">
    <h4>✓ Best For</h4>
    <ul>
      <li><strong>Serious runners</strong> who need advanced training metrics</li>
      <li><strong>Triathletes</strong> requiring multi-sport tracking</li>
      <li><strong>Data enthusiasts</strong> who want detailed analytics</li>
      <li><strong>Long-distance athletes</strong> needing extended battery</li>
    </ul>
  </div>
  <div class="should-skip">
    <h4>✗ Skip If</h4>
    <ul>
      <li>You're a casual fitness user (overkill features)</li>
      <li>Budget is under $400</li>
      <li>You prefer smaller watch sizes</li>
      <li>You don't use training plans</li>
    </ul>
  </div>
</div>
```

### Final Verdict Box
```html
<div class="final-verdict">
  <div class="verdict-score">
    <span class="score-large">9.2</span>
    <span class="score-label">Excellent</span>
  </div>
  <div class="verdict-breakdown">
    <div class="breakdown-item">
      <span class="item-name">Performance</span>
      <span class="item-score">9.5</span>
    </div>
    <div class="breakdown-item">
      <span class="item-name">Features</span>
      <span class="item-score">9.0</span>
    </div>
    <div class="breakdown-item">
      <span class="item-name">Value</span>
      <span class="item-score">8.0</span>
    </div>
    <div class="breakdown-item">
      <span class="item-name">Design</span>
      <span class="item-score">9.0</span>
    </div>
  </div>
  <div class="verdict-summary">
    <p>The [Product] earns our highest recommendation for [target audience]. 
    Despite [minor weakness], the [key strength] makes it the best choice 
    in its category.</p>
  </div>
  <div class="verdict-cta">
    <a href="#" class="btn-primary">Check Price on Amazon</a>
    <a href="#" class="btn-secondary">Compare Alternatives</a>
  </div>
</div>
```

---

## n8n Content Workflows

### Review Update Workflow
```
Trigger: Weekly
→ Get all published reviews
→ Check product availability (PAAPI)
→ Compare current price vs published
→ If price changed >5%:
   → Update price in post
   → Add "Price Updated" notice
→ If out of stock:
   → Add "Currently Unavailable" notice
```

### New Product Alert Workflow
```
Trigger: RSS feeds from tech sites
→ Filter for product announcements
→ Match against our categories
→ If match:
   → Create Notion task
   → Assign for review consideration
```

---

## Files Reference

```
tech-review-templates/
├── SKILL.md (this file)
├── templates/
│   ├── single-review-page.php
│   ├── best-of-roundup.php
│   ├── versus-comparison.php
│   └── gutenberg-blocks/
├── components/
│   ├── quick-verdict.html
│   ├── specs-table.html
│   ├── who-should-buy.html
│   ├── final-verdict.html
│   ├── fitness-metrics.html
│   ├── health-sensors.html
│   └── ecosystem-matrix.html
├── css/
│   ├── review-base.css
│   ├── review-pulsegear.css
│   ├── review-wearable.css
│   └── review-smarthome.css
└── n8n/
    ├── review-update-workflow.json
    └── new-product-alert.json
```
