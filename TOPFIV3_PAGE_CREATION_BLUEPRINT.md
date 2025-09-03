# TopFiv3 Page Creation Blueprint

## 🚨 CRITICAL RULES - NO EXCEPTIONS

### Research Requirements
- **MUST research EACH product on the web BEFORE writing ANY content**
- **NO fabricating product information under any circumstances** 
- Use only factual, verified specifications and features
- Write content that sounds human and natural, not AI-generated
- Cross-reference multiple sources for accuracy

### Image Requirements  
- **DO NOT create your own images - EVER**
- User personally places ALL images in correct folders
- Find existing images and verify correct filenames BEFORE building pages
- If images cannot be found, NOTIFY USER they are missing
- Image paths: `../../images/products/` for product images, `../../images/reviews/` for banners

### File Naming Conventions
- Top 5 pages: `category-name-2025.html` 
- Individual reviews: `product-brand-model-review.html` (lowercase, hyphens)
- Use proper product names in titles, NOT model numbers

---

## TOP 5 RANKING PAGE STRUCTURE

### Required Order:
1. **HTML Head** (SEO meta tags, structured data, fonts)
2. **Breadcrumbs** (Home > Category > Page Name)
3. **Hero Banner** (Category-specific banner image)
4. **Intro Section** (Brief description paragraph)
5. **Top 3 Spotlight** (Grid layout with #1, #2, #3 picks)
6. **Quick Compare Table** (Specs comparison with review links)
7. **Products 4 & 5 ONLY** (Remaining products listed in product-list section)
8. **CTA Section** (Category return link - "Explore [Category] Rankings")
9. **Disclosure** (Affiliate disclaimer)

### Example Structure (from cordless-drill-impact-combos-2025.html):
```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Top 5 Cordless Drill & Impact Driver Combos of 2025 | TopFiv3</title>
<meta name="description" content="We tested 2025's best cordless drill and impact driver combo kits for power, battery life, and value. See our ranked Top 5 and the 3 combos that are truly worth your money.">
<meta name="keywords" content="best cordless drill combo 2025, DEWALT combo kit, Milwaukee FUEL combo, drill impact driver combo, cordless tool reviews, brushless drill combo">

<!-- Canonical URL -->
<link rel="canonical" href="https://topfiv3.com/reviews/diy/cordless-drill-impact-combos-2025.html">

<!-- Breadcrumbs (SEO) -->
<script type="application/ld+json">
{
  "@context":"https://schema.org",
  "@type":"BreadcrumbList",
  "itemListElement":[
    {"@type":"ListItem","position":1,"name":"Home","item":"https://topfiv3.com/"},
    {"@type":"ListItem","position":2,"name":"DIY & Tools","item":"https://topfiv3.com/diy-tools.html"},
    {"@type":"ListItem","position":3,"name":"Cordless Drill & Impact Combos 2025"}
  ]
}
</script>

<!-- ItemList (Top 5) -->
<script type="application/ld+json">
{
  "@context":"https://schema.org",
  "@type":"ItemList",
  "name":"Top 5 Cordless Drill & Impact Driver Combos of 2025",
  "itemListElement":[
    {"@type":"ListItem","position":1,"url":"https://topfiv3.com/reviews/diy/products/dewalt-dck240c2-review.html","name":"DEWALT 20V MAX Combo Kit DCK240C2"},
    {"@type":"ListItem","position":2,"url":"https://topfiv3.com/reviews/diy/products/milwaukee-2997-22-review.html","name":"Milwaukee M18 FUEL Combo Kit 2997-22"},
    {"@type":"ListItem","position":3,"url":"https://topfiv3.com/reviews/diy/products/craftsman-cmck200c2am-review.html","name":"CRAFTSMAN V20 MAX Combo Kit CMCK200C2AM"},
    {"@type":"ListItem","position":4,"url":"https://topfiv3.com/reviews/diy/products/dewalt-dck299m2-review.html","name":"DEWALT 20V MAX Hammer Drill Combo DCK299M2"},
    {"@type":"ListItem","position":5,"url":"https://topfiv3.com/reviews/diy/products/makita-ct225syx-review.html","name":"Makita 18V LXT Combo Kit CT225SYX"}
  ]
}
</script>

<style>
  :root{
    --bg:#f3f4f6; --card:#fff; --ink:#111827; --muted:#6b7280;
    --brand:#f59e0b; --cta:#ff2d55; --ring:rgba(245,158,11,.35);
    --radius:14px;
  }
  /* [CSS continues...] */
</style>
</head>
<body>

<div class="breadcrumbs">
  <a href="../../index.html">Home</a> > 
  <a href="../../diy-tools.html">DIY & Tools</a> > 
  <span>Cordless Drill Combos 2025</span>
</div>

<div class="ranking-hero">
  <h1>Top 5 Cordless Drill & Impact Driver Combos of 2025</h1>
</div>

<div class="intro">
  <p>We tested 15+ cordless drill and impact driver combo kits from major brands, evaluating power delivery, battery life, build quality, and overall value. These 5 represent the best combinations of performance and price, with 3 clear winners that dominate their respective categories.</p>
</div>

<div id="top3" class="top3-spotlight">
  <div class="item">
    <img src="../../images/products/dewaltdck240c2.jpg" alt="DEWALT 20V MAX Cordless Drill and Impact Driver Combo Kit">
    <span class="tag">#1 Best Value</span>
    <h3>DEWALT 20V MAX Cordless Drill and Impact Driver Combo Kit</h3>
    <p>Reliable brushed motors with 300 UWO power, compact design, and two 1.3Ah batteries. Perfect entry-level combo for DIYers and basic home projects with proven DEWALT quality.</p>
    <a href="https://amzn.to/4g3kSlq" target="_blank" rel="nofollow">Buy on Amazon</a>
    <a href="products/dewalt-dck240c2-review.html">Read Full Review</a>
  </div>
  <!-- Continue with items #2 and #3 -->
</div>

<div id="compare" class="compare">
  <h2>Quick Compare</h2>
  <div class="table-wrap">
    <table>
      <thead>
        <tr>
          <th>Product</th>
          <th>Motor Type</th>
          <th>Power Output</th>
          <th>Battery</th>
          <th>Special Features</th>
          <th>Review</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td><strong>DEWALT 20V MAX Combo Kit</strong></td>
          <td>Brushed</td>
          <td>300 UWO / 1,500 RPM</td>
          <td>2x 1.3Ah</td>
          <td>Compact design, LED lights</td>
          <td><a href="products/dewalt-dck240c2-review.html">Review</a></td>
        </tr>
        <!-- Continue with other products -->
      </tbody>
    </table>
  </div>
</div>

<div class="product-list">
  <div class="product">
    <img src="../../images/products/dewaltdck299m2.jpg" alt="DEWALT 20V MAX XR Brushless Hammer Drill Combo Kit">
    <div class="product-info">
      <h4>#4 – DEWALT 20V MAX XR Brushless Hammer Drill Combo Kit</h4>
      <p>Heavy-duty combo with hammer function for masonry work, brushless motors, and high torque output (1,825 in-lbs). Includes two 4.0Ah batteries for extended runtime on demanding jobs.</p>
      <div class="product-cta">
        <a href="https://amzn.to/3UVyPbC" target="_blank" rel="nofollow">Buy on Amazon</a>
        <a href="products/dewalt-dck299m2-review.html">Read Full Review</a>
      </div>
    </div>
  </div>
  
  <div class="product">
    <!-- Product #5 only -->
  </div>
</div>

<div class="cta-section">
  Want more DIY & tools product reviews? Visit the full <strong>DIY & Tools</strong> category for top picks, deep dives, and expert recommendations.
  <br>
  <a href="../../diy-tools.html">Explore DIY & Tools Rankings</a>
</div>

<div class="disclaimer">
  <em>Disclosure:</em> This page contains affiliate links. We may earn a commission if you click and make a purchase — at no additional cost to you. This helps support our work. Thank you!
</div>

</body>
</html>
```

---

## INDIVIDUAL REVIEW PAGE STRUCTURE

### Required Order (CORRECTED):
1. **HTML Head** (Product-specific SEO meta tags)
2. **Breadcrumbs** (Home > Category > Subcategory > Product Name) 
3. **Hero Banner** (Product-specific banner image)
4. **Back Link** (Return to category page)
5. **Quick Product Summary** (1-2 sentence overview paragraph)
6. **🚨 EMBOLDENED REVIEW SCORE** (Rating highlight box - THIS COMES AFTER SUMMARY)
7. **Review Content** (Detailed sections covering features, performance, etc.)
8. **Pros & Cons** (Side-by-side layout)
9. **Specifications Table** (Technical details)
10. **Buy Button** (Amazon affiliate link)
11. **Final Verdict** (Summary conclusion box)
12. **Affiliate Disclaimer**

### Example Structure (from asus-rtx-5070-smart-buy-review.html):
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ASUS RTX 5070 Smart Buy Review 2025 - Below MSRP Graphics Card Deal | TopFiv3</title>
    <meta name="description" content="ASUS Prime RTX 5070 12GB GDDR7 review at $523.79 - below MSRP pricing with DLSS 4, Blackwell architecture, and SFF-Ready design. Exceptional value buy.">
    <meta name="keywords" content="ASUS RTX 5070 review, RTX 5070 below MSRP, graphics card deal, DLSS 4, Blackwell architecture, SFF-Ready GPU, value graphics card 2025">
    
    <!-- Canonical URL -->
    <link rel="canonical" href="https://topfiv3.com/reviews/misc/asus-rtx-5070-smart-buy-review.html">
</head>
<body>

<div class="breadcrumbs">
  <a href="../../index.html">Home</a> > 
  <a href="../../misc-smart-buys.html">Misc & Smart Buys</a> > 
  <span>ASUS RTX 5070 Smart Buy Review</span>
</div>

<div class="review-hero">
  ASUS RTX 5070 Smart Buy Review
</div>

<div class="back-link">
  <a href="../../misc-smart-buys.html">← Back to Misc & Smart Buys</a>
</div>

<div class="review-container">
  <!-- 🚨 QUICK PRODUCT SUMMARY FIRST -->
  <p>The ASUS Prime GeForce RTX 5070 12GB GDDR7 represents an exceptional smart buy in today's inflated GPU market, offering cutting-edge Blackwell architecture with DLSS 4 technology at a price below MSRP when most RTX 50-series cards are selling above retail.</p>

  <!-- 🚨 THEN EMBOLDENED RATING/PRICE HIGHLIGHT -->
  <div class="price-highlight">
    <h3>🔥 Smart Buy Alert</h3>
    <div class="current-price">$523.79</div>
    <span class="original-price">$609.99</span>
    <div class="savings">Save $86.20 - Below MSRP Pricing!</div>
  </div>

  <!-- DETAILED REVIEW CONTENT -->
  <h2>NVIDIA Blackwell Architecture & DLSS 4</h2>
  <p>Powered by the revolutionary 5nm Blackwell architecture with 6,144 CUDA cores and 988 TOPs of AI performance...</p>

  <!-- PROS & CONS -->
  <h2>Pros & Cons</h2>
  <div class="pros-cons">
    <div class="pros">
      <h3>✅ Pros</h3>
      <ul>
        <li>Below MSRP pricing ($523.79 vs $549 MSRP)</li>
        <li>Cutting-edge DLSS 4 with Multi-Frame Generation</li>
      </ul>
    </div>
    <div class="cons">
      <h3>⚠️ Cons</h3>
      <ul>
        <li>Limited availability at this price point</li>
      </ul>
    </div>
  </div>

  <!-- SPECIFICATIONS TABLE -->
  <h2>Specifications</h2>
  <table class="specs-table">
    <tr><th>Feature</th><th>Details</th></tr>
    <tr><td>GPU Architecture</td><td>NVIDIA Blackwell (5nm)</td></tr>
  </table>

  <!-- BUY BUTTON -->
  <a href="https://amzn.to/example" class="buy-button" target="_blank" rel="nofollow">Buy on Amazon</a>

  <!-- FINAL VERDICT -->
  <div class="final-verdict">
    <h2>Final Verdict</h2>
    <p>This represents a rare opportunity to access cutting-edge graphics technology at a price that actually saves money...</p>
  </div>

  <!-- AFFILIATE DISCLAIMER -->
  <div class="disclaimer">
    <em>Disclosure:</em> This page contains affiliate links. We may earn a commission if you click and make a purchase — at no additional cost to you. This helps support our work. Thank you!
  </div>
</div>

</body>
</html>
```

---

## MAIN CATEGORY PAGE TEASER FORMAT (Standard Categories)

### Structure (from diy-tools.html):
```html
<div class="section">
  <div class="teaser-grid">
    <div class="teaser-block">
      <img src="images/teasers/top5cordlessdrillimpactteaser.png" alt="Top 5 Cordless Drill & Impact Driver Combos 2025">
      <div class="teaser-content">
        <div class="teaser-title">Top 5 Cordless Drill & Impact Driver Combos 2025</div>
        <div class="teaser-desc">
          We tested 15+ combo kits from DEWALT, Milwaukee, CRAFTSMAN, and Makita. From budget picks to professional-grade powerhouses, discover the top 3 combos that deliver the best value.
        </div>
        <a href="reviews/diy/cordless-drill-impact-combos-2025.html" class="teaser-link">View Rankings</a>
      </div>
    </div>
  </div>
</div>
```

### Required CSS Classes (Standard Categories):
- `.section` - Main container
- `.teaser-grid` - Grid container (2-column on desktop)
- `.teaser-block` - Individual teaser card
- `.teaser-content` - Text content wrapper
- `.teaser-title` - Ranking page title
- `.teaser-desc` - Brief description
- `.teaser-link` - Rankings link ("View Rankings")

---

## MISC CATEGORY PAGE TEASER FORMAT (Special Format)

### Structure (from misc-smart-buys.html):
```html
<div class="teaser-grid">
  <div class="teaser-block">
    <img src="images/products/asusrtx5070.jpg" alt="ASUS RTX 5070">
    <div class="teaser-content">
      <div class="teaser-title">ASUS RTX 5070 Smart Buy</div>
      <div class="teaser-description">Below MSRP pricing on cutting-edge Blackwell GPU with DLSS 4 and 12GB GDDR7. Rare opportunity at $523.79 - save $86 vs MSRP.</div>
      <a href="reviews/misc/asus-rtx-5070-smart-buy-review.html" class="teaser-link">Read Review →</a>
    </div>
  </div>
</div>
```

### Required CSS Classes (MISC Only):
- `.teaser-grid` - Grid container
- `.teaser-block` - Individual teaser card  
- `.teaser-content` - Text content wrapper
- `.teaser-title` - Product name
- `.teaser-description` - Brief description (different class name!)
- `.teaser-link` - Review link ("Read Review →")

---

## CSS STYLING REQUIREMENTS

### Color Schemes by Category:
- **DIY & Tools**: Orange theme (`--brand:#f59e0b`)
- **Tech**: Green theme (`--brand:#10b981`) 
- **Home**: Blue theme (varies by page)
- **Misc**: Yellow theme (`background: #fefce8`)

### Required CSS Classes:
- `.breadcrumbs` - Navigation breadcrumbs
- `.ranking-hero` / `.review-hero` - Hero banner sections
- `.intro` - Intro paragraph section
- `.top3-spotlight` - Top 3 products grid
- `.item` - Individual spotlight item
- `.tag` - Ranking tags (#1, #2, #3)
- `.compare` - Comparison table section
- `.table-wrap` - Table wrapper
- `.product-list` - Products 4&5 section
- `.product` - Individual product block
- `.product-info` - Product text content
- `.product-cta` - Button container
- `.rating-highlight` / `.price-highlight` - Emboldened score/price section
- `.pros-cons` - Pros/cons container
- `.pros` / `.cons` - Individual columns
- `.specs-table` - Specifications table
- `.buy-button` - Amazon purchase button
- `.final-verdict` - Conclusion section
- `.cta-section` - Category return section
- `.back-link` - Return to category link
- `.disclaimer` - Affiliate disclosure

---

## PRE-CREATION CHECKLIST

### Before Writing ANY Content:
- [ ] Research ALL products on the web for accurate specifications
- [ ] Verify ALL image files exist in correct folders with proper filenames
- [ ] Confirm Amazon affiliate links are provided
- [ ] Check category color scheme and CSS variables
- [ ] Prepare proper product names (not model numbers) for titles

### File Structure Verification:
- [ ] Product images: `images/products/[product-name].jpg`
- [ ] Banner images: `images/reviews/[banner-name].png` 
- [ ] Teaser images: `images/teasers/[teaser-name].png` (for standard categories)
- [ ] Review files: `reviews/[category]/products/[product-review].html`
- [ ] Top 5 files: `reviews/[category]/[category-name]-2025.html`

### Content Requirements:
- [ ] Human-sounding, natural language 
- [ ] Factual specifications only
- [ ] Proper SEO meta tags and structured data
- [ ] Consistent CSS classes and styling
- [ ] All affiliate disclosures included
- [ ] **ADD TEASER TO MAIN CATEGORY PAGE** (e.g., tech-electronics.html, diy-tools.html)
- [ ] If unsure which main category page, ASK FOR CLARIFICATION before proceeding

---

## POST-CREATION REQUIREMENTS (BEFORE PUSHING TO GITHUB)

### MANDATORY Final Steps:
- [ ] **ADD TEASER TO MAIN CATEGORY PAGE** - Replace "Coming Soon" or add new teaser block
- [ ] **UPDATE SITEMAP.XML** - Add ALL new pages with current date
- [ ] **VERIFY SEO OPTIMIZATION** - Meta descriptions, keywords, structured data
- [ ] **CHECK ALL LINKS** - Amazon affiliates, internal review links, category returns
- [ ] **VALIDATE HTML** - Proper closing tags, CSS class consistency
- [ ] **TEST RESPONSIVENESS** - Mobile/desktop layout verification

### Sitemap.xml Update Format:
```xml
<!-- Category Review Pages -->
<url>
  <loc>https://topfiv3.com/reviews/[category]/[page-name]-2025.html</loc>
  <lastmod>2025-09-02</lastmod>
  <changefreq>monthly</changefreq>
  <priority>0.8</priority>
</url>

<!-- Individual Product Review Pages -->
<url>
  <loc>https://topfiv3.com/reviews/[category]/products/[product-review].html</loc>
  <lastmod>2025-09-02</lastmod>
  <changefreq>monthly</changefreq>
  <priority>0.7</priority>
</url>
```

### SEO Optimization Checklist:
- [ ] Title includes year (2025) and "TopFiv3"
- [ ] Meta description under 160 characters with key benefits
- [ ] Keywords include product names, category terms, year
- [ ] **CANONICAL TAG REQUIRED** - Add `<link rel="canonical" href="https://topfiv3.com/[page-path]">` after keywords
- [ ] Structured data (JSON-LD) for breadcrumbs and item lists
- [ ] Alt attributes on all images
- [ ] Heading hierarchy (H1 → H2 → H3)

**⚠️ NO PUSHING TO GITHUB WITHOUT SITEMAP UPDATE AND SEO VERIFICATION**

This blueprint ensures 100% consistency with established TopFiv3 page formats and prevents the formatting errors encountered previously.