---
title: Technical SEO Audit - Example.com
date: 2025-11-21
site_url: https://example.com
tools_used: [Screaming Frog, Google Search Console, PageSpeed Insights]
audit_type: quarterly
---

# Technical SEO Audit - Example.com

## Executive Summary

**Site:** https://example.com
**Audit Date:** 2025-11-21
**Pages Crawled:** 1,250
**Critical Issues:** 5
**Warnings:** 23
**Notices:** 47

**Overall Health Score:** 72/100 (Good, needs improvement)

## Critical Issues (Fix Immediately)

### 1. Duplicate Content (25 pages)

**Issue:** Product pages have duplicate descriptions
**Impact:** Keyword cannibalization, wasted crawl budget
**Affected URLs:** [List or file]

**Fix:**
- Rewrite product descriptions (unique for each)
- Add canonical tags to variant pages
- Use noindex for true duplicates

**Priority:** HIGH
**Estimated time:** 2 weeks

### 2. Broken Internal Links (42 instances)

**Issue:** Links pointing to deleted or moved pages
**Impact:** Poor user experience, crawl errors
**Affected pages:** [List]

**Fix:**
- Update links to correct URLs
- Implement proper 301 redirects
- Set up monitoring for future breaks

**Priority:** HIGH
**Estimated time:** 2 days

### 3. Mobile Usability Errors (15 pages)

**Issue:** Text too small, buttons too close, content wider than screen
**Impact:** Mobile rankings penalty
**Affected URLs:** [List]

**Fix:**
- Increase font size (min 16px)
- Add spacing between tap targets
- Fix horizontal scroll issues

**Priority:** HIGH
**Estimated time:** 1 week

### 4. Missing XML Sitemap

**Issue:** No sitemap submitted to Google Search Console
**Impact:** Slower indexing, missed pages

**Fix:**
- Generate XML sitemap
- Submit to GSC
- Add sitemap reference to robots.txt

**Priority:** HIGH
**Estimated time:** 1 hour

### 5. Slow Page Speed (Multiple pages)

**Issue:** Pages loading in 5-8 seconds on mobile
**Impact:** High bounce rate, ranking penalty
**Core Web Vitals:** FAIL

**Fix:**
- Optimize images (WebP format, lazy loading)
- Minify CSS/JS
- Enable compression
- Implement browser caching

**Priority:** HIGH
**Estimated time:** 1 week

## Warnings (Fix Soon)

### Missing Meta Descriptions (18 pages)

**Impact:** Lower CTR from SERP
**Fix:** Write unique descriptions (150-160 chars)
**Priority:** MEDIUM

### Thin Content (12 pages)

**Impact:** Low quality signals to Google
**Fix:** Expand content to 500+ words or noindex
**Priority:** MEDIUM

### Missing Alt Text (85 images)

**Impact:** Accessibility issues, missed image search traffic
**Fix:** Add descriptive alt text to all images
**Priority:** MEDIUM

### H1 Issues (Multiple H1s or Missing)

**Impact:** Confuses search engines about page topic
**Fix:** Ensure one H1 per page, use H2-H6 for structure
**Priority:** MEDIUM

## Notices (Monitor)

### Redirect Chains (8 instances)

**Example:** URL A → 301 → URL B → 301 → URL C
**Fix:** Redirect directly from A to C
**Priority:** LOW

### External Links (5 broken)

**Fix:** Update or remove broken external links
**Priority:** LOW

## Page Speed Analysis

### Desktop
- **Performance:** 85/100 (Good)
- **Accessibility:** 92/100 (Good)
- **Best Practices:** 88/100 (Good)
- **SEO:** 95/100 (Good)

### Mobile
- **Performance:** 62/100 (Needs Improvement)
- **Accessibility:** 90/100 (Good)
- **Best Practices:** 85/100 (Good)
- **SEO:** 93/100 (Good)

**Main bottlenecks:**
- Large image files (1-3MB each)
- Render-blocking JavaScript
- No browser caching
- Too many HTTP requests

## Core Web Vitals

| Metric | Desktop | Mobile | Status |
|--------|---------|--------|--------|
| LCP (Largest Contentful Paint) | 2.1s | 3.8s | FAIL (mobile) |
| FID (First Input Delay) | 45ms | 120ms | PASS |
| CLS (Cumulative Layout Shift) | 0.05 | 0.12 | PASS |

**Target:** LCP < 2.5s, FID < 100ms, CLS < 0.1

## Indexing Status

**Google Search Console:**
- Total indexed pages: 980
- Total submitted pages: 1,250
- Coverage issues: 270 pages

**Common issues:**
- "Crawled - currently not indexed" (150 pages)
- "Discovered - currently not indexed" (80 pages)
- "Excluded by robots.txt" (40 pages)

## Schema Markup

**Current implementation:**
- ✅ Organization schema (homepage)
- ✅ Product schema (product pages)
- ❌ Article schema (blog posts) - MISSING
- ❌ BreadcrumbList schema - MISSING
- ❌ FAQ schema - MISSING

**Recommendations:**
- Add Article schema to all blog posts
- Implement BreadcrumbList for better SERP display
- Add FAQ schema to pages with Q&A sections

## Mobile Optimization

**Issues found:**
- Some images not responsive
- Pop-ups block content on mobile
- Font size too small on product pages
- Buttons too small (less than 48x48px)

**Fixes:**
- Use responsive images (srcset)
- Adjust pop-up timing/size
- Increase font to 16px minimum
- Enlarge tap targets to 48x48px minimum

## Security

✅ HTTPS enabled (SSL certificate valid)
✅ No mixed content warnings
✅ Secure cookies (httpOnly, secure flags)

## Robots.txt Review

```
User-agent: *
Disallow: /admin/
Disallow: /cart/
Disallow: /checkout/
Sitemap: https://example.com/sitemap.xml
```

**Recommendations:**
- ✅ Properly blocks admin areas
- ✅ Sitemap referenced
- ⚠️ Consider blocking /search/ pages

## Action Plan

### Week 1 (High Priority)
- [ ] Fix broken internal links
- [ ] Generate and submit XML sitemap
- [ ] Add missing meta descriptions

### Week 2-3 (High Priority)
- [ ] Optimize images (compress, WebP, lazy load)
- [ ] Fix mobile usability errors
- [ ] Minify CSS/JS

### Week 4 (Medium Priority)
- [ ] Rewrite duplicate product descriptions
- [ ] Add missing alt text
- [ ] Implement Article schema

### Ongoing (Monitor)
- [ ] Track Core Web Vitals monthly
- [ ] Check GSC for new coverage issues
- [ ] Run quarterly technical audits

---

**Tools used:**
- Screaming Frog SEO Spider
- Google Search Console
- Google PageSpeed Insights
- GTmetrix
- Schema.org validator

**Next audit:** 2026-02-21 (3 months)

**Related files:**
- Previous audit: [2025-08-site-audit.md](2025-08-site-audit.md)
- Page speed fixes: [page-speed-optimization.md](page-speed-optimization.md)
