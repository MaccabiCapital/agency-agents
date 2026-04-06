# Workflow: Campaign Landing Page Sprint

> Build a conversion-optimized landing page for a local service business in one day using 4 agents.

## Scenario

A dental practice is running Google Ads and needs a landing page for "teeth whitening [city]." The page needs to load fast, capture leads, and route them into GHL for automated follow-up.

## Agent Team

| Agent | Role in This Sprint |
|-------|-------------------|
| UX Architect | Wireframe the page structure and conversion flow |
| UI Designer | Visual design with dental practice branding |
| Website & Landing Page Developer | Build the page, connect forms to GHL |
| Reality Checker | QA the page before ads point to it |

## Workflow

### Step 1: UX Architect (1-2 hours)
- Review the ad copy and keyword targets
- Wireframe the landing page: headline → trust signals → service details → CTA → form
- Specify mobile layout (60-70% of traffic will be mobile)
- Output: annotated wireframe with CTA placement and form fields

### Step 2: UI Designer (2-3 hours)
- Apply dental practice brand (logo, colors, fonts)
- Design desktop and mobile mockups from wireframe
- Select/create hero image and trust signal elements
- Output: design mockups ready for development

### Step 3: Website & Landing Page Developer (3-4 hours)
- Build the page in GHL or standalone HTML
- Connect form to GHL pipeline with UTM pass-through
- Implement tracking: GTM, GA4 event, Google Ads conversion tag
- Optimize for speed: compress images, minimize scripts, target LCP < 2.5s
- Set up thank-you page with next steps

### Step 4: Reality Checker (1-2 hours)
- Submit test form and verify data arrives in GHL
- Check mobile rendering on 3 device sizes
- Verify tracking fires correctly (GTM debug mode)
- Run PageSpeed Insights and verify Core Web Vitals pass
- Verdict: APPROVED or NEEDS WORK with specific defects

## Quality Gate
Page does not receive ad traffic until Reality Checker issues APPROVED verdict with:
- Form submission proof (GHL contact screenshot)
- Mobile screenshot evidence
- PageSpeed Insights passing score
- Tracking verification (GTM debug screenshot)

## Total Time: 6-10 hours across 4 agents
