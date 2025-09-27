# SolLaunch - Updated Frontend Code

## File Structure:
```
sollaunch-platform/
├── index.html
├── style.css
├── app.js
├── README.md
└── assets/
    ├── logo_3d.png
    ├── hero_3d.png
    ├── phases_3d.png
    ├── revenue_3d.png
    └── network_3d.png
```

## Deployment Instructions for GitHub + Vercel:

### Step 1: Create GitHub Repository
1. Go to GitHub.com and sign in with username: solbanz352
2. Click "New Repository" 
3. Name: "sollaunch-platform"
4. Make it Public
5. Initialize with README
6. Click "Create Repository"

### Step 2: Upload Files
1. Click "uploading an existing file" on your new repo
2. Drag and drop all the files provided below
3. Commit changes with message: "Initial SolLaunch platform deployment"

### Step 3: Deploy on Vercel
1. Go to vercel.com and sign up/login
2. Click "New Project"
3. Import your GitHub repo: solbanz352/sollaunch-platform
4. Click "Deploy"
5. Your live URL will be generated automatically!

### Step 4: Custom Domain (Optional)
1. In Vercel dashboard, go to your project
2. Click "Domains" tab
3. Add your custom domain (e.g., sollaunch.com)

## Files to Upload:

### index.html
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SolLaunch - Stop Guessing. Start Validating. Transform Your SaaS Idea into Revenue in Weeks.</title>
    <meta name="description" content="Join the elite founders who pre-sell first, build smart, and scale fast with SolLaunch. Elite Validation Program starting October 15th - Limited to 8 participants.">
    
    <!-- Open Graph / Facebook -->
    <meta property="og:type" content="website">
    <meta property="og:url" content="https://sollaunch.com/">
    <meta property="og:title" content="SolLaunch - Transform Your SaaS Idea into Revenue in Weeks">
    <meta property="og:description" content="Stop building products nobody wants. Join elite founders who validate first, build smart, and scale fast.">
    <meta property="og:image" content="https://user-gen-media-assets.s3.amazonaws.com/seedream_images/961dcf09-79d5-4dc0-9803-954bb98fbc89.png">

    <!-- Twitter -->
    <meta property="twitter:card" content="summary_large_image">
    <meta property="twitter:url" content="https://sollaunch.com/">
    <meta property="twitter:title" content="SolLaunch - Transform Your SaaS Idea into Revenue in Weeks">
    <meta property="twitter:description" content="Stop building products nobody wants. Join elite founders who validate first, build smart, and scale fast.">
    <meta property="twitter:image" content="https://user-gen-media-assets.s3.amazonaws.com/seedream_images/961dcf09-79d5-4dc0-9803-954bb98fbc89.png">
    
    <link rel="stylesheet" href="style.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
</head>
<body>
    <!-- Navigation -->
    <nav class="nav" id="navbar">
        <div class="nav-container">
            <div class="nav-logo">
                <img src="https://user-gen-media-assets.s3.amazonaws.com/seedream_images/961dcf09-79d5-4dc0-9803-954bb98fbc89.png" alt="SolLaunch 3D Logo - Elite SaaS Validation Platform" class="logo-img">
            </div>
            <div class="nav-links">
                <a href="#hero" class="nav-link">Home</a>
                <a href="#problem" class="nav-link">Problem</a>
                <a href="#process" class="nav-link">Process</a>
                <a href="#pricing" class="nav-link">Pricing</a>
                <a href="#success" class="nav-link">Success Stories</a>
                <button class="btn btn--primary nav-cta" onclick="openModal('applicationModal')">Apply Now to Save Your Spot</button>
            </div>
            <div class="nav-toggle" id="nav-toggle">
                <span></span>
                <span></span>
                <span></span>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="hero" class="hero">
        <div class="hero-container">
            <div class="hero-content">
                <div class="hero-text">
                    <div class="hero-logo-large">
                        <img src="https://user-gen-media-assets.s3.amazonaws.com/seedream_images/961dcf09-79d5-4dc0-9803-954bb98fbc89.png" alt="SolLaunch 3D Logo Large" class="hero-logo-img">
                    </div>
                    <h1 class="hero-title">Stop Guessing. Start Validating.<br>Transform Your SaaS Idea into Revenue in <span class="highlight">Weeks</span>.</h1>
                    <p class="hero-subtitle">Join the elite founders who pre-sell first, build smart, and scale fast with SolLaunch.</p>
                    
                    <!-- Benefits Bullets -->
                    <div class="hero-benefits">
                        <div class="benefit">
                            <span class="benefit-icon">✓</span>
                            <span>Validate your SaaS idea with <strong>real pre-sales revenue</strong> before building</span>
                        </div>
                        <div class="benefit">
                            <span class="benefit-icon">✓</span>
                            <span>Partner with expert developers invested in your success</span>
                        </div>
                        <div class="benefit">
                            <span class="benefit-icon">✓</span>
                            <span>Access exclusive investor showcases and an elite founders community</span>
                        </div>
                    </div>
                    
                    <div class="hero-cta">
                        <button class="btn btn--primary btn--lg" onclick="openModal('applicationModal')">Apply Now to Save Your Spot</button>
                        <button class="btn btn--outline btn--lg" onclick="openModal('consultationModal')">Schedule Your Free Strategy Call</button>
                    </div>
                    
                    <!-- Countdown Timer -->
                    <div class="countdown">
                        <h3>Next Elite Cohort Launches:</h3>
                        <div class="countdown-timer">
                            <div class="countdown-item">
                                <span id="days" class="countdown-number">18</span>
                                <span class="countdown-label">Days</span>
                            </div>
                            <div class="countdown-item">
                                <span id="hours" class="countdown-number">06</span>
                                <span class="countdown-label">Hours</span>
                            </div>
                            <div class="countdown-item">
                                <span id="minutes" class="countdown-number">42</span>
                                <span class="countdown-label">Minutes</span>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="hero-visual">
                    <img src="https://user-gen-media-assets.s3.amazonaws.com/seedream_images/710491b3-b7c1-49cf-ab78-19f988b8e351.png" alt="3D Holographic SaaS Validation Dashboard Interface" class="hero-img parallax-element">
                </div>
            </div>
        </div>
    </section>

    <!-- Problem Section -->
    <section id="problem" class="problem">
        <div class="container">
            <div class="problem-content">
                <h2 class="section-title">The Harsh Reality of SaaS Failures</h2>
                <div class="problem-stat">
                    <span class="stat-number">72%</span>
                    <p class="stat-text">of SaaS startups fail within the first two years—not from bad code, but from building the wrong product for the wrong market.</p>
                </div>
                
                <div class="comparison-grid">
                    <div class="comparison-item comparison-item--traditional">
                        <h3>Traditional Founders Follow This Path to Failure:</h3>
                        <ul>
                            <li>Build for months based on assumptions</li>
                            <li>Launch to crickets</li>
                            <li>Burn through savings</li>
                            <li>Pivot too late</li>
                            <li>Give up</li>
                        </ul>
                    </div>
                    <div class="comparison-item comparison-item--sollaunch">
                        <h3>SolLaunch Founders Take a Different Path:</h3>
                        <ul>
                            <li>Validate through real revenue first</li>
                            <li>Build what customers already want to buy</li>
                            <li>Partner with aligned development experts</li>
                            <li>Scale with proven investor connections</li>
                            <li>Succeed with 89% success rate</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Process Section -->
    <section id="process" class="process">
        <div class="container">
            <h2 class="section-title">Our Battle-Tested 3-Phase Framework</h2>
            <div class="process-visual">
                <img src="https://user-gen-media-assets.s3.amazonaws.com/seedream_images/da449dfa-f761-4f9e-87fe-7097fbe50c99.png" alt="3D Metallic Process Phases: VALIDATE, BUILD, SCALE connected by teal energy beams" class="process-img parallax-element">
            </div>
            <div class="phases-grid">
                <div class="phase-card" data-phase="validate">
                    <div class="phase-header">
                        <h3>Phase 1: VALIDATE</h3>
                        <p class="phase-subtitle">Prove Market Demand Before You Build</p>
                        <p class="phase-duration">Duration: 3-4 weeks intensive validation sprint</p>
                    </div>
                    <div class="phase-content">
                        <p>Transform untested assumptions into validated opportunities through our proprietary pre-sales methodology.</p>
                        <h4>What You'll Accomplish:</h4>
                        <ul>
                            <li>Generate your first $5K-$25K in pre-sales without any product</li>
                            <li>Build compelling value propositions that convert prospects to pre-sales</li>
                            <li>Execute advanced market validation techniques beyond surveys</li>
                            <li>Access real customer insights to guide development decisions</li>
                        </ul>
                    </div>
                </div>
                
                <div class="phase-card" data-phase="build">
                    <div class="phase-header">
                        <h3>Phase 2: BUILD</h3>
                        <p class="phase-subtitle">Develop With Strategic Partners</p>
                        <p class="phase-duration">For validated ideas showing $10K+ pre-sale potential</p>
                    </div>
                    <div class="phase-content">
                        <p>Unlike traditional development shops, we become invested partners in your success.</p>
                        <h4>Our Partnership Model:</h4>
                        <ul>
                            <li>Small equity stake (3-7%) aligned with your success</li>
                            <li>Significantly reduced development costs (50-70% below market)</li>
                            <li>Revenue-focused development roadmap</li>
                            <li>Built-in scalability and best practices from day one</li>
                        </ul>
                    </div>
                </div>
                
                <div class="phase-card" data-phase="scale">
                    <div class="phase-header">
                        <h3>Phase 3: SCALE</h3>
                        <p class="phase-subtitle">Connect With Elite Growth Capital</p>
                        <p class="phase-duration">Bi-annual exclusive investor showcases</p>
                    </div>
                    <div class="phase-content">
                        <p>Present your validated, revenue-generating SaaS to pre-vetted investors with $5M+ investment capacity.</p>
                        <h4>Elite Growth Showcase Benefits:</h4>
                        <ul>
                            <li>Pitch to investors specifically seeking early-stage SaaS opportunities</li>
                            <li>Professional pitch coaching and deck optimization</li>
                            <li>Network with growth-stage capital sources</li>
                            <li>Receive strategic feedback from industry veterans</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Features Section -->
    <section id="features" class="features">
        <div class="container">
            <h2 class="section-title">Why SolLaunch Delivers Results</h2>
            <div class="features-grid">
                <div class="feature-card">
                    <div class="feature-visual">
                        <img src="https://user-gen-media-assets.s3.amazonaws.com/seedream_images/0a91b1d1-0b27-4929-9507-1a2306546ecc.png" alt="3D Holographic Revenue Growth Chart with teal neon accents" class="feature-img">
                    </div>
                    <h3>Revenue-First Validation</h3>
                    <p>Skip the guesswork. Validate through actual pre-sales and paying customers before investing significant development resources.</p>
                </div>
                
                <div class="feature-card">
                    <h3>Aligned Success Partnership</h3>
                    <p>Our unique equity model means we succeed only when you succeed—creating true partnership alignment versus transactional relationships.</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-visual">
                        <img src="https://user-gen-media-assets.s3.amazonaws.com/seedream_images/6de182cc-b8db-4240-8acb-a21249a2d219.png" alt="3D Metallic Network Nodes representing Elite Founders Circle community" class="feature-img">
                    </div>
                    <h3>Elite Founder Network</h3>
                    <p>Access an exclusive community of revenue-validated entrepreneurs facing similar challenges and sharing proven strategies.</p>
                </div>
                
                <div class="feature-card">
                    <h3>Technical Excellence Without Debt</h3>
                    <p>Leverage enterprise-grade development expertise while maintaining focus on customer development and market expansion.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Pricing Section -->
    <section id="pricing" class="pricing">
        <div class="container">
            <h2 class="section-title">Join Our Next Elite Validation Cohort</h2>
            <div class="pricing-card">
                <div class="pricing-header">
                    <h3>Elite Validation Program</h3>
                    <div class="price">
                        <span class="currency">$</span>
                        <span class="amount">4,997</span>
                    </div>
                </div>
                <div class="pricing-content">
                    <h4>Program Structure:</h4>
                    <ul class="pricing-features">
                        <li>3-4 week intensive validation sprint</li>
                        <li>Lifetime Elite Founders Circle membership</li>
                        <li>2 one-on-one strategy sessions with SaaS veterans</li>
                        <li>Weekly group coaching and accountability calls</li>
                        <li>Access to our complete validation toolkit</li>
                    </ul>
                    
                    <div class="pricing-guarantees">
                        <div class="guarantee">
                            <strong>30-day money-back guarantee</strong> (no questions asked)
                        </div>
                        <div class="guarantee">
                            Payment plans available
                        </div>
                        <div class="guarantee">
                            Next cohort launches <strong>October 15th</strong> - limited to <strong>8 participants</strong>
                        </div>
                    </div>
                    
                    <div class="pricing-cta">
                        <button class="btn btn--primary btn--lg" onclick="openModal('applicationModal')">Apply Now to Save Your Spot</button>
                        <button class="btn btn--outline" onclick="openModal('consultationModal')">Schedule Strategy Call</button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Success Stories Section -->
    <section id="success" class="success">
        <div class="container">
            <h2 class="section-title">Success Stories</h2>
            <div class="success-stats">
                <div class="stat">
                    <span class="stat-number">89%</span>
                    <span class="stat-label">Success Rate for Validated Ideas</span>
                </div>
                <div class="stat">
                    <span class="stat-number">$18K</span>
                    <span class="stat-label">Average Pre-Sales in 3 Weeks</span>
                </div>
                <div class="stat">
                    <span class="stat-number">200+</span>
                    <span class="stat-label">Elite Founders Transformed</span>
                </div>
            </div>
            
            <div class="testimonials-grid">
                <div class="testimonial-card">
                    <div class="testimonial-content">
                        <p>"I generated $18K in pre-sales in 3 weeks using SolLaunch's framework. That validation gave me the confidence to quit my job and build full-time."</p>
                    </div>
                    <div class="testimonial-author">
                        <strong>Sarah Chen</strong>
                        <span>Founder of DataSync Pro</span>
                    </div>
                </div>
                
                <div class="testimonial-card">
                    <div class="testimonial-content">
                        <p>"The partner development model saved me 8 months and $75K compared to traditional agencies. More importantly, we built exactly what our pre-sale customers wanted."</p>
                    </div>
                    <div class="testimonial-author">
                        <strong>Marcus Rodriguez</strong>
                        <span>CEO of FlowOps</span>
                    </div>
                </div>
                
                <div class="testimonial-card">
                    <div class="testimonial-content">
                        <p>"From validated idea to $50K MRR in 7 months. The investor connections alone were worth 10x the program cost."</p>
                    </div>
                    <div class="testimonial-author">
                        <strong>Jennifer Kim</strong>
                        <span>Founder of TeamAlign</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- FAQ Section -->
    <section id="faq" class="faq">
        <div class="container">
            <h2 class="section-title">Frequently Asked Questions</h2>
            <div class="faq-grid">
                <div class="faq-item">
                    <div class="faq-question" onclick="toggleFAQ(this)">
                        <h3>How is this different from other startup programs?</h3>
                        <span class="faq-toggle">+</span>
                    </div>
                    <div class="faq-answer">
                        <p>We focus exclusively on revenue validation before building. Most programs teach you to build and hope. We teach you to sell first, then build what buyers want.</p>
                    </div>
                </div>
                
                <div class="faq-item">
                    <div class="faq-question" onclick="toggleFAQ(this)">
                        <h3>What if my idea doesn't validate?</h3>
                        <span class="faq-toggle">+</span>
                    </div>
                    <div class="faq-answer">
                        <p>Better to know in 3 weeks than after 6 months of development. We'll help you pivot to a validated opportunity or refund your investment.</p>
                    </div>
                </div>
                
                <div class="faq-item">
                    <div class="faq-question" onclick="toggleFAQ(this)">
                        <h3>Do you take equity in the validation phase?</h3>
                        <span class="faq-toggle">+</span>
                    </div>
                    <div class="faq-answer">
                        <p>No. Equity partnerships only begin if you choose our BUILD phase for validated ideas with strong pre-sale traction.</p>
                    </div>
                </div>
                
                <div class="faq-item">
                    <div class="faq-question" onclick="toggleFAQ(this)">
                        <h3>What industries do you work with?</h3>
                        <span class="faq-toggle">+</span>
                    </div>
                    <div class="faq-answer">
                        <p>We specialize in B2B SaaS across all verticals. Our methods work for any software solution that solves business problems.</p>
                    </div>
                </div>
                
                <div class="faq-item">
                    <div class="faq-question" onclick="toggleFAQ(this)">
                        <h3>Can I validate without technical skills?</h3>
                        <span class="faq-toggle">+</span>
                    </div>
                    <div class="faq-answer">
                        <p>Absolutely. Our validation methods require no coding. We provide all templates, scripts, and frameworks needed.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="footer">
        <div class="container">
            <div class="footer-content">
                <div class="footer-logo">
                    <img src="https://user-gen-media-assets.s3.amazonaws.com/seedream_images/961dcf09-79d5-4dc0-9803-954bb98fbc89.png" alt="SolLaunch Logo" class="footer-logo-img">
                </div>
                <div class="footer-links">
                    <a href="#" class="footer-link">Terms</a>
                    <a href="#" class="footer-link">Privacy</a>
                    <a href="#" class="footer-link">Contact</a>
                </div>
            </div>
            <div class="footer-bottom">
                <p>&copy; 2025 SolLaunch. All rights reserved. Join the elite founders who validate first, build smart, and scale fast.</p>
            </div>
        </div>
    </footer>

    <!-- Application Modal -->
    <div id="applicationModal" class="modal">
        <div class="modal-content">
            <span class="modal-close" onclick="closeModal('applicationModal')">&times;</span>
            <h2>Apply for Elite Validation Program</h2>
            <form class="application-form">
                <div class="form-group">
                    <label for="name">Full Name *</label>
                    <input type="text" id="name" name="name" required>
                </div>
                <div class="form-group">
                    <label for="email">Email Address *</label>
                    <input type="email" id="email" name="email" required>
                </div>
                <div class="form-group">
                    <label for="company">Company/Startup Name</label>
                    <input type="text" id="company" name="company">
                </div>
                <div class="form-group">
                    <label for="idea">Brief Description of Your SaaS Idea *</label>
                    <textarea id="idea" name="idea" rows="4" required></textarea>
                </div>
                <div class="form-group">
                    <label for="experience">Previous Startup/Business Experience</label>
                    <textarea id="experience" name="experience" rows="3"></textarea>
                </div>
                <div class="form-group">
                    <label for="commitment">Why are you committed to this validation process? *</label>
                    <textarea id="commitment" name="commitment" rows="3" required></textarea>
                </div>
                <button type="submit" class="btn btn--primary btn--lg">Submit Application</button>
            </form>
        </div>
    </div>

    <!-- Consultation Modal -->
    <div id="consultationModal" class="modal">
        <div class="modal-content">
            <span class="modal-close" onclick="closeModal('consultationModal')">&times;</span>
            <h2>Schedule Your Free Strategy Call</h2>
            <form class="consultation-form">
                <div class="form-group">
                    <label for="consult-name">Full Name *</label>
                    <input type="text" id="consult-name" name="name" required>
                </div>
                <div class="form-group">
                    <label for="consult-email">Email Address *</label>
                    <input type="email" id="consult-email" name="email" required>
                </div>
                <div class="form-group">
                    <label for="consult-phone">Phone Number</label>
                    <input type="tel" id="consult-phone" name="phone">
                </div>
                <div class="form-group">
                    <label for="consult-stage">What stage is your SaaS idea? *</label>
                    <select id="consult-stage" name="stage" required>
                        <option value="">Select stage...</option>
                        <option value="concept">Just a concept/idea</option>
                        <option value="research">Did some market research</option>
                        <option value="mockup">Have mockups/wireframes</option>
                        <option value="prototype">Built a prototype</option>
                        <option value="launched">Already launched</option>
                    </select>
                </div>
                <div class="form-group">
                    <label for="consult-challenge">What's your biggest challenge right now? *</label>
                    <textarea id="consult-challenge" name="challenge" rows="3" required></textarea>
                </div>
                <button type="submit" class="btn btn--primary btn--lg">Schedule Free Call</button>
            </form>
        </div>
    </div>

    <script src="app.js"></script>
</body>
</html>
```

### style.css
```css
/* Reset and Base Styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

:root {
    /* Color Palette */
    --primary-dark: #0a0a0a;
    --secondary-dark: #1a1a1a;
    --metallic-gray: #2a2a2a;
    --teal-neon: #00ffcc;
    --teal-secondary: #00d4aa;
    --white: #ffffff;
    --gray-text: #cccccc;
    --gray-light: #666666;
    
    /* Typography */
    --font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
    --font-size-xs: 0.75rem;
    --font-size-sm: 0.875rem;
    --font-size-base: 1rem;
    --font-size-lg: 1.125rem;
    --font-size-xl: 1.25rem;
    --font-size-2xl: 1.5rem;
    --font-size-3xl: 1.875rem;
    --font-size-4xl: 2.25rem;
    --font-size-5xl: 3rem;
    
    /* Spacing */
    --spacing-xs: 0.25rem;
    --spacing-sm: 0.5rem;
    --spacing-base: 1rem;
    --spacing-lg: 1.5rem;
    --spacing-xl: 2rem;
    --spacing-2xl: 3rem;
    --spacing-3xl: 4rem;
    
    /* Transitions */
    --transition-fast: 0.15s ease-in-out;
    --transition-base: 0.3s ease-in-out;
    --transition-slow: 0.5s ease-in-out;
}

body {
    font-family: var(--font-family);
    line-height: 1.6;
    color: var(--white);
    background: linear-gradient(135deg, var(--primary-dark) 0%, var(--secondary-dark) 100%);
    overflow-x: hidden;
}

/* Smooth Scrolling */
html {
    scroll-behavior: smooth;
}

/* Container */
.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 var(--spacing-xl);
}

/* Navigation */
.nav {
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    background: rgba(10, 10, 10, 0.95);
    backdrop-filter: blur(10px);
    border-bottom: 1px solid rgba(0, 255, 204, 0.2);
    z-index: 1000;
    transition: var(--transition-base);
}

.nav-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: var(--spacing-base) var(--spacing-xl);
    max-width: 1200px;
    margin: 0 auto;
}

.nav-logo .logo-img {
    height: 40px;
    width: auto;
    filter: drop-shadow(0 0 10px var(--teal-neon));
}

.nav-links {
    display: flex;
    align-items: center;
    gap: var(--spacing-xl);
}

.nav-link {
    color: var(--gray-text);
    text-decoration: none;
    font-weight: 500;
    transition: var(--transition-base);
    position: relative;
}

.nav-link:hover {
    color: var(--teal-neon);
}

.nav-link::after {
    content: '';
    position: absolute;
    bottom: -5px;
    left: 0;
    width: 0;
    height: 2px;
    background: var(--teal-neon);
    transition: var(--transition-base);
}

.nav-link:hover::after {
    width: 100%;
}

.nav-toggle {
    display: none;
    flex-direction: column;
    cursor: pointer;
}

.nav-toggle span {
    width: 25px;
    height: 3px;
    background: var(--teal-neon);
    margin: 3px 0;
    transition: var(--transition-base);
}

/* Buttons */
.btn {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    padding: var(--spacing-base) var(--spacing-xl);
    border: none;
    border-radius: 8px;
    font-family: var(--font-family);
    font-weight: 600;
    text-decoration: none;
    cursor: pointer;
    transition: var(--transition-base);
    position: relative;
    overflow: hidden;
}

.btn--primary {
    background: linear-gradient(45deg, var(--teal-neon), var(--teal-secondary));
    color: var(--primary-dark);
    box-shadow: 0 0 20px rgba(0, 255, 204, 0.3);
}

.btn--primary:hover {
    transform: translateY(-2px);
    box-shadow: 0 5px 25px rgba(0, 255, 204, 0.5);
}

.btn--outline {
    background: transparent;
    color: var(--teal-neon);
    border: 2px solid var(--teal-neon);
}

.btn--outline:hover {
    background: var(--teal-neon);
    color: var(--primary-dark);
    box-shadow: 0 0 20px rgba(0, 255, 204, 0.3);
}

.btn--lg {
    padding: var(--spacing-lg) var(--spacing-2xl);
    font-size: var(--font-size-lg);
}

/* Hero Section */
.hero {
    min-height: 100vh;
    display: flex;
    align-items: center;
    position: relative;
    padding-top: 80px;
}

.hero-container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 var(--spacing-xl);
}

.hero-content {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: var(--spacing-3xl);
    align-items: center;
}

.hero-logo-large {
    margin-bottom: var(--spacing-xl);
}

.hero-logo-img {
    height: 80px;
    width: auto;
    filter: drop-shadow(0 0 20px var(--teal-neon));
}

.hero-title {
    font-size: var(--font-size-5xl);
    font-weight: 700;
    line-height: 1.1;
    margin-bottom: var(--spacing-xl);
    background: linear-gradient(135deg, var(--white) 0%, var(--teal-neon) 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
}

.highlight {
    color: var(--teal-neon);
    text-shadow: 0 0 10px var(--teal-neon);
}

.hero-subtitle {
    font-size: var(--font-size-xl);
    color: var(--gray-text);
    margin-bottom: var(--spacing-2xl);
    line-height: 1.6;
}

.hero-benefits {
    margin-bottom: var(--spacing-2xl);
}

.benefit {
    display: flex;
    align-items: flex-start;
    gap: var(--spacing-base);
    margin-bottom: var(--spacing-base);
}

.benefit-icon {
    color: var(--teal-neon);
    font-weight: bold;
    font-size: var(--font-size-lg);
    margin-top: 2px;
}

.hero-cta {
    display: flex;
    gap: var(--spacing-lg);
    margin-bottom: var(--spacing-2xl);
    flex-wrap: wrap;
}

.hero-visual {
    display: flex;
    justify-content: center;
    align-items: center;
}

.hero-img {
    width: 100%;
    max-width: 500px;
    height: auto;
    filter: drop-shadow(0 0 30px rgba(0, 255, 204, 0.3));
}

/* Countdown Timer */
.countdown {
    background: rgba(42, 42, 42, 0.5);
    border: 1px solid rgba(0, 255, 204, 0.3);
    border-radius: 12px;
    padding: var(--spacing-xl);
    text-align: center;
}

.countdown h3 {
    color: var(--teal-neon);
    margin-bottom: var(--spacing-base);
    font-size: var(--font-size-lg);
}

.countdown-timer {
    display: flex;
    justify-content: center;
    gap: var(--spacing-xl);
}

.countdown-item {
    display: flex;
    flex-direction: column;
    align-items: center;
}

.countdown-number {
    font-size: var(--font-size-3xl);
    font-weight: 700;
    color: var(--teal-neon);
    text-shadow: 0 0 10px var(--teal-neon);
}

.countdown-label {
    font-size: var(--font-size-sm);
    color: var(--gray-text);
    text-transform: uppercase;
    letter-spacing: 1px;
}

/* Section Styles */
section {
    padding: var(--spacing-3xl) 0;
}

.section-title {
    font-size: var(--font-size-4xl);
    font-weight: 700;
    text-align: center;
    margin-bottom: var(--spacing-3xl);
    background: linear-gradient(135deg, var(--white) 0%, var(--teal-neon) 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
}

/* Problem Section */
.problem {
    background: rgba(26, 26, 26, 0.5);
}

.problem-stat {
    text-align: center;
    margin-bottom: var(--spacing-3xl);
}

.stat-number {
    font-size: 6rem;
    font-weight: 900;
    color: var(--teal-neon);
    text-shadow: 0 0 20px var(--teal-neon);
    display: block;
}

.stat-text {
    font-size: var(--font-size-xl);
    color: var(--gray-text);
    max-width: 800px;
    margin: 0 auto;
    line-height: 1.6;
}

.comparison-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: var(--spacing-2xl);
    margin-top: var(--spacing-3xl);
}

.comparison-item {
    background: rgba(42, 42, 42, 0.5);
    border-radius: 12px;
    padding: var(--spacing-2xl);
    border: 1px solid rgba(255, 255, 255, 0.1);
}

.comparison-item--traditional {
    border-color: rgba(255, 84, 89, 0.3);
}

.comparison-item--sollaunch {
    border-color: rgba(0, 255, 204, 0.3);
    background: rgba(0, 255, 204, 0.05);
}

.comparison-item h3 {
    margin-bottom: var(--spacing-lg);
    font-size: var(--font-size-xl);
}

.comparison-item ul {
    list-style: none;
}

.comparison-item li {
    margin-bottom: var(--spacing-base);
    padding-left: var(--spacing-lg);
    position: relative;
}

.comparison-item--traditional li::before {
    content: "✗";
    position: absolute;
    left: 0;
    color: #ff5459;
}

.comparison-item--sollaunch li::before {
    content: "✓";
    position: absolute;
    left: 0;
    color: var(--teal-neon);
}

/* Process Section */
.process-visual {
    text-align: center;
    margin-bottom: var(--spacing-3xl);
}

.process-img {
    width: 100%;
    max-width: 800px;
    height: auto;
    filter: drop-shadow(0 0 30px rgba(0, 255, 204, 0.2));
}

.phases-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
    gap: var(--spacing-2xl);
}

.phase-card {
    background: rgba(42, 42, 42, 0.5);
    border: 1px solid rgba(0, 255, 204, 0.3);
    border-radius: 16px;
    padding: var(--spacing-2xl);
    transition: var(--transition-base);
    position: relative;
    overflow: hidden;
}

.phase-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 4px;
    background: linear-gradient(90deg, var(--teal-neon), var(--teal-secondary));
}

.phase-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 30px rgba(0, 255, 204, 0.2);
}

.phase-header h3 {
    font-size: var(--font-size-2xl);
    color: var(--teal-neon);
    margin-bottom: var(--spacing-sm);
}

.phase-subtitle {
    font-size: var(--font-size-lg);
    color: var(--white);
    margin-bottom: var(--spacing-sm);
    font-weight: 600;
}

.phase-duration {
    color: var(--gray-text);
    font-style: italic;
    margin-bottom: var(--spacing-lg);
}

.phase-content h4 {
    color: var(--teal-neon);
    margin: var(--spacing-lg) 0 var(--spacing-base) 0;
}

.phase-content ul {
    list-style: none;
}

.phase-content li {
    margin-bottom: var(--spacing-sm);
    padding-left: var(--spacing-lg);
    position: relative;
}

.phase-content li::before {
    content: "▶";
    position: absolute;
    left: 0;
    color: var(--teal-neon);
}

/* Features Section */
.features-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: var(--spacing-2xl);
}

.feature-card {
    background: rgba(42, 42, 42, 0.5);
    border: 1px solid rgba(255, 255, 255, 0.1);
    border-radius: 12px;
    padding: var(--spacing-2xl);
    text-align: center;
    transition: var(--transition-base);
}

.feature-card:hover {
    border-color: rgba(0, 255, 204, 0.5);
    transform: translateY(-3px);
}

.feature-visual {
    margin-bottom: var(--spacing-lg);
}

.feature-img {
    width: 100%;
    max-width: 200px;
    height: auto;
    filter: drop-shadow(0 0 20px rgba(0, 255, 204, 0.3));
}

.feature-card h3 {
    font-size: var(--font-size-xl);
    margin-bottom: var(--spacing-base);
    color: var(--teal-neon);
}

/* Pricing Section */
.pricing {
    background: rgba(26, 26, 26, 0.5);
}

.pricing-card {
    max-width: 600px;
    margin: 0 auto;
    background: rgba(42, 42, 42, 0.8);
    border: 2px solid var(--teal-neon);
    border-radius: 20px;
    padding: var(--spacing-3xl);
    position: relative;
    overflow: hidden;
}

.pricing-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 6px;
    background: linear-gradient(90deg, var(--teal-neon), var(--teal-secondary));
}

.pricing-header {
    text-align: center;
    margin-bottom: var(--spacing-2xl);
}

.pricing-header h3 {
    font-size: var(--font-size-2xl);
    margin-bottom: var(--spacing-base);
}

.price {
    display: flex;
    justify-content: center;
    align-items: baseline;
    gap: var(--spacing-sm);
}

.currency {
    font-size: var(--font-size-2xl);
    color: var(--teal-neon);
}

.amount {
    font-size: 4rem;
    font-weight: 900;
    color: var(--teal-neon);
    text-shadow: 0 0 15px var(--teal-neon);
}

.pricing-features {
    list-style: none;
    margin-bottom: var(--spacing-2xl);
}

.pricing-features li {
    margin-bottom: var(--spacing-base);
    padding-left: var(--spacing-lg);
    position: relative;
}

.pricing-features li::before {
    content: "✓";
    position: absolute;
    left: 0;
    color: var(--teal-neon);
    font-weight: bold;
}

.pricing-guarantees {
    background: rgba(0, 255, 204, 0.1);
    border: 1px solid rgba(0, 255, 204, 0.3);
    border-radius: 8px;
    padding: var(--spacing-lg);
    margin-bottom: var(--spacing-2xl);
}

.guarantee {
    margin-bottom: var(--spacing-sm);
    text-align: center;
}

.guarantee:last-child {
    margin-bottom: 0;
}

.pricing-cta {
    display: flex;
    flex-direction: column;
    gap: var(--spacing-base);
}

/* Success Section */
.success-stats {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: var(--spacing-2xl);
    margin-bottom: var(--spacing-3xl);
}

.stat {
    text-align: center;
    padding: var(--spacing-xl);
    background: rgba(42, 42, 42, 0.5);
    border-radius: 12px;
    border: 1px solid rgba(0, 255, 204, 0.3);
}

.stat-number {
    font-size: var(--font-size-4xl);
    font-weight: 900;
    color: var(--teal-neon);
    text-shadow: 0 0 15px var(--teal-neon);
    display: block;
    margin-bottom: var(--spacing-sm);
}

.stat-label {
    color: var(--gray-text);
    font-size: var(--font-size-sm);
    text-transform: uppercase;
    letter-spacing: 1px;
}

.testimonials-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: var(--spacing-xl);
}

.testimonial-card {
    background: rgba(42, 42, 42, 0.5);
    border: 1px solid rgba(255, 255, 255, 0.1);
    border-radius: 12px;
    padding: var(--spacing-2xl);
    position: relative;
}

.testimonial-card::before {
    content: '"';
    font-size: 4rem;
    color: var(--teal-neon);
    position: absolute;
    top: var(--spacing-base);
    left: var(--spacing-base);
    opacity: 0.3;
}

.testimonial-content {
    margin-bottom: var(--spacing-lg);
    padding-top: var(--spacing-lg);
}

.testimonial-author strong {
    color: var(--teal-neon);
    display: block;
}

.testimonial-author span {
    color: var(--gray-text);
    font-size: var(--font-size-sm);
}

/* FAQ Section */
.faq-grid {
    max-width: 800px;
    margin: 0 auto;
}

.faq-item {
    border: 1px solid rgba(255, 255, 255, 0.1);
    border-radius: 8px;
    margin-bottom: var(--spacing-base);
    overflow: hidden;
}

.faq-question {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: var(--spacing-lg);
    background: rgba(42, 42, 42, 0.5);
    cursor: pointer;
    transition: var(--transition-base);
}

.faq-question:hover {
    background: rgba(0, 255, 204, 0.1);
}

.faq-question h3 {
    font-size: var(--font-size-lg);
    font-weight: 600;
}

.faq-toggle {
    font-size: var(--font-size-xl);
    color: var(--teal-neon);
    transition: var(--transition-base);
}

.faq-item.active .faq-toggle {
    transform: rotate(45deg);
}

.faq-answer {
    padding: 0 var(--spacing-lg);
    max-height: 0;
    overflow: hidden;
    transition: var(--transition-base);
    background: rgba(26, 26, 26, 0.5);
}

.faq-item.active .faq-answer {
    padding: var(--spacing-lg);
    max-height: 200px;
}

/* Footer */
.footer {
    background: var(--primary-dark);
    border-top: 1px solid rgba(0, 255, 204, 0.2);
    padding: var(--spacing-2xl) 0;
}

.footer-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: var(--spacing-lg);
}

.footer-logo-img {
    height: 30px;
    width: auto;
    filter: drop-shadow(0 0 10px var(--teal-neon));
}

.footer-links {
    display: flex;
    gap: var(--spacing-xl);
}

.footer-link {
    color: var(--gray-text);
    text-decoration: none;
    transition: var(--transition-base);
}

.footer-link:hover {
    color: var(--teal-neon);
}

.footer-bottom {
    text-align: center;
    color: var(--gray-text);
    font-size: var(--font-size-sm);
    border-top: 1px solid rgba(255, 255, 255, 0.1);
    padding-top: var(--spacing-lg);
}

/* Modals */
.modal {
    display: none;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0, 0, 0, 0.8);
    backdrop-filter: blur(5px);
    z-index: 2000;
    animation: fadeIn 0.3s ease-in-out;
}

.modal.active {
    display: flex;
    align-items: center;
    justify-content: center;
}

@keyframes fadeIn {
    from { opacity: 0; }
    to { opacity: 1; }
}

.modal-content {
    background: var(--secondary-dark);
    border: 2px solid var(--teal-neon);
    border-radius: 16px;
    padding: var(--spacing-2xl);
    max-width: 600px;
    width: 90%;
    max-height: 90vh;
    overflow-y: auto;
    position: relative;
    animation: slideIn 0.3s ease-in-out;
}

@keyframes slideIn {
    from {
        transform: translateY(-50px);
        opacity: 0;
    }
    to {
        transform: translateY(0);
        opacity: 1;
    }
}

.modal-close {
    position: absolute;
    top: var(--spacing-base);
    right: var(--spacing-lg);
    font-size: var(--font-size-2xl);
    color: var(--gray-text);
    cursor: pointer;
    transition: var(--transition-base);
}

.modal-close:hover {
    color: var(--teal-neon);
}

.modal h2 {
    margin-bottom: var(--spacing-xl);
    color: var(--teal-neon);
}

/* Forms */
.form-group {
    margin-bottom: var(--spacing-lg);
}

.form-group label {
    display: block;
    margin-bottom: var(--spacing-sm);
    font-weight: 600;
    color: var(--white);
}

.form-group input,
.form-group select,
.form-group textarea {
    width: 100%;
    padding: var(--spacing-base);
    border: 2px solid rgba(255, 255, 255, 0.2);
    border-radius: 8px;
    background: rgba(42, 42, 42, 0.5);
    color: var(--white);
    font-family: var(--font-family);
    font-size: var(--font-size-base);
    transition: var(--transition-base);
}

.form-group input:focus,
.form-group select:focus,
.form-group textarea:focus {
    outline: none;
    border-color: var(--teal-neon);
    box-shadow: 0 0 10px rgba(0, 255, 204, 0.3);
}

/* Parallax Elements */
.parallax-element {
    transition: transform 0.1s ease-out;
}

/* Responsive Design */
@media (max-width: 768px) {
    .nav-links {
        display: none;
        position: absolute;
        top: 100%;
        left: 0;
        right: 0;
        background: rgba(10, 10, 10, 0.95);
        flex-direction: column;
        padding: var(--spacing-xl);
        gap: var(--spacing-base);
    }
    
    .nav-links.active {
        display: flex;
    }
    
    .nav-toggle {
        display: flex;
    }
    
    .hero-content {
        grid-template-columns: 1fr;
        text-align: center;
    }
    
    .hero-title {
        font-size: var(--font-size-3xl);
    }
    
    .hero-cta {
        flex-direction: column;
    }
    
    .comparison-grid {
        grid-template-columns: 1fr;
    }
    
    .countdown-timer {
        gap: var(--spacing-base);
    }
    
    .countdown-number {
        font-size: var(--font-size-2xl);
    }
    
    .phases-grid {
        grid-template-columns: 1fr;
    }
    
    .pricing-cta {
        align-items: stretch;
    }
    
    .footer-content {
        flex-direction: column;
        gap: var(--spacing-base);
        text-align: center;
    }
}

@media (max-width: 480px) {
    .container {
        padding: 0 var(--spacing-base);
    }
    
    .hero-title {
        font-size: var(--font-size-2xl);
    }
    
    .section-title {
        font-size: var(--font-size-2xl);
    }
    
    .stat-number {
        font-size: 4rem;
    }
    
    .amount {
        font-size: 3rem;
    }
}

/* Animation Classes */
.fade-in {
    animation: fadeInUp 0.6s ease-out forwards;
    opacity: 0;
    transform: translateY(30px);
}

@keyframes fadeInUp {
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

.slide-in-left {
    animation: slideInLeft 0.6s ease-out forwards;
    opacity: 0;
    transform: translateX(-30px);
}

@keyframes slideInLeft {
    to {
        opacity: 1;
        transform: translateX(0);
    }
}

.slide-in-right {
    animation: slideInRight 0.6s ease-out forwards;
    opacity: 0;
    transform: translateX(30px);
}

@keyframes slideInRight {
    to {
        opacity: 1;
        transform: translateX(0);
    }
}

/* Utility Classes */
.text-center {
    text-align: center;
}

.text-gradient {
    background: linear-gradient(135deg, var(--white) 0%, var(--teal-neon) 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
}

.glow {
    filter: drop-shadow(0 0 10px var(--teal-neon));
}
```

### app.js
```javascript
// SolLaunch Application JavaScript
document.addEventListener('DOMContentLoaded', function() {
    // Initialize all components
    initCountdown();
    initScrollAnimations();
    initSmoothScrolling();
    initMobileNav();
    initParallax();
    
    // Set up event listeners
    setupEventListeners();
});

// Countdown Timer Functionality
function initCountdown() {
    const targetDate = new Date('October 15, 2025 00:00:00').getTime();
    
    function updateCountdown() {
        const now = new Date().getTime();
        const timeLeft = targetDate - now;
        
        if (timeLeft > 0) {
            const days = Math.floor(timeLeft / (1000 * 60 * 60 * 24));
            const hours = Math.floor((timeLeft % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
            const minutes = Math.floor((timeLeft % (1000 * 60 * 60)) / (1000 * 60));
            
            const daysElement = document.getElementById('days');
            const hoursElement = document.getElementById('hours');
            const minutesElement = document.getElementById('minutes');
            
            if (daysElement) daysElement.textContent = days.toString().padStart(2, '0');
            if (hoursElement) hoursElement.textContent = hours.toString().padStart(2, '0');
            if (minutesElement) minutesElement.textContent = minutes.toString().padStart(2, '0');
        } else {
            const daysElement = document.getElementById('days');
            const hoursElement = document.getElementById('hours');
            const minutesElement = document.getElementById('minutes');
            
            if (daysElement) daysElement.textContent = '00';
            if (hoursElement) hoursElement.textContent = '00';
            if (minutesElement) minutesElement.textContent = '00';
        }
    }
    
    // Update immediately and then every minute
    updateCountdown();
    setInterval(updateCountdown, 60000);
}

// Smooth Scrolling Navigation
function initSmoothScrolling() {
    const navLinks = document.querySelectorAll('.nav-link[href^="#"]');
    
    navLinks.forEach(link => {
        link.addEventListener('click', function(e) {
            e.preventDefault();
            const targetId = this.getAttribute('href').substring(1);
            const targetSection = document.getElementById(targetId);
            
            if (targetSection) {
                const navHeight = document.querySelector('.nav').offsetHeight;
                const targetPosition = targetSection.offsetTop - navHeight - 20;
                
                window.scrollTo({
                    top: targetPosition,
                    behavior: 'smooth'
                });
                
                // Close mobile nav if open
                const navLinks = document.querySelector('.nav-links');
                if (navLinks.classList.contains('active')) {
                    navLinks.classList.remove('active');
                }
            }
        });
    });
}

// Mobile Navigation
function initMobileNav() {
    const navToggle = document.getElementById('nav-toggle');
    const navLinks = document.querySelector('.nav-links');
    
    if (navToggle && navLinks) {
        navToggle.addEventListener('click', function() {
            navLinks.classList.toggle('active');
        });
        
        // Close nav when clicking outside
        document.addEventListener('click', function(e) {
            if (!navToggle.contains(e.target) && !navLinks.contains(e.target)) {
                navLinks.classList.remove('active');
            }
        });
    }
}

// Scroll Animations
function initScrollAnimations() {
    const observerOptions = {
        threshold: 0.1,
        rootMargin: '0px 0px -50px 0px'
    };
    
    const observer = new IntersectionObserver(function(entries) {
        entries.forEach(entry => {
            if (entry.isIntersecting) {
                entry.target.classList.add('fade-in');
            }
        });
    }, observerOptions);
    
    // Observe elements for animation
    const animateElements = document.querySelectorAll('.phase-card, .feature-card, .testimonial-card, .stat');
    animateElements.forEach(el => observer.observe(el));
}

// Parallax Effect
function initParallax() {
    window.addEventListener('scroll', function() {
        const scrolled = window.pageYOffset;
        const parallaxElements = document.querySelectorAll('.parallax-element');
        
        parallaxElements.forEach(element => {
            const speed = 0.5;
            const yPos = -(scrolled * speed);
            element.style.transform = `translateY(${yPos}px)`;
        });
    });
}

// Modal Functions
function openModal(modalId) {
    const modal = document.getElementById(modalId);
    if (modal) {
        modal.classList.add('active');
        document.body.style.overflow = 'hidden';
    }
}

function closeModal(modalId) {
    const modal = document.getElementById(modalId);
    if (modal) {
        modal.classList.remove('active');
        document.body.style.overflow = 'auto';
    }
}

// FAQ Toggle
function toggleFAQ(element) {
    const faqItem = element.parentElement;
    const answer = faqItem.querySelector('.faq-answer');
    
    faqItem.classList.toggle('active');
    
    if (faqItem.classList.contains('active')) {
        answer.style.maxHeight = answer.scrollHeight + 'px';
    } else {
        answer.style.maxHeight = '0';
    }
}

// Form Submissions
function setupEventListeners() {
    // Application Form
    const applicationForm = document.querySelector('.application-form');
    if (applicationForm) {
        applicationForm.addEventListener('submit', function(e) {
            e.preventDefault();
            
            // Get form data
            const formData = new FormData(this);
            const data = Object.fromEntries(formData);
            
            // Validate required fields
            if (!data.name || !data.email || !data.idea || !data.commitment) {
                alert('Please fill in all required fields.');
                return;
            }
            
            // Show success message
            alert('Thank you for your application! We will review it and get back to you within 24 hours.');
            
            // Close modal and reset form
            closeModal('applicationModal');
            this.reset();
            
            // In a real application, you would send this data to your backend
            console.log('Application submitted:', data);
        });
    }
    
    // Consultation Form
    const consultationForm = document.querySelector('.consultation-form');
    if (consultationForm) {
        consultationForm.addEventListener('submit', function(e) {
            e.preventDefault();
            
            // Get form data
            const formData = new FormData(this);
            const data = Object.fromEntries(formData);
            
            // Validate required fields
            if (!data.name || !data.email || !data.stage || !data.challenge) {
                alert('Please fill in all required fields.');
                return;
            }
            
            // Show success message
            alert('Thank you for scheduling a call! We will send you a calendar link within 2 hours.');
            
            // Close modal and reset form
            closeModal('consultationModal');
            this.reset();
            
            // In a real application, you would send this data to your backend
            console.log('Consultation scheduled:', data);
        });
    }
    
    // Close modals when clicking outside
    document.addEventListener('click', function(e) {
        if (e.target.classList.contains('modal')) {
            closeModal(e.target.id);
        }
    });
    
    // Close modals with Escape key
    document.addEventListener('keydown', function(e) {
        if (e.key === 'Escape') {
            const activeModals = document.querySelectorAll('.modal.active');
            activeModals.forEach(modal => {
                closeModal(modal.id);
            });
        }
    });
}

// Sticky Navigation
window.addEventListener('scroll', function() {
    const nav = document.querySelector('.nav');
    if (window.scrollY > 100) {
        nav.style.background = 'rgba(10, 10, 10, 0.98)';
    } else {
        nav.style.background = 'rgba(10, 10, 10, 0.95)';
    }
});

// Page Load Performance
window.addEventListener('load', function() {
    // Hide loading spinner if you have one
    const loader = document.querySelector('.loader');
    if (loader) {
        loader.style.display = 'none';
    }
    
    // Initialize any additional animations
    const heroElements = document.querySelectorAll('.hero .fade-in');
    heroElements.forEach((el, index) => {
        setTimeout(() => {
            el.classList.add('fade-in');
        }, index * 200);
    });
});

// Error Handling
window.addEventListener('error', function(e) {
    console.error('JavaScript error:', e.error);
    // In production, you might want to send this to an error tracking service
});

// Utility Functions
function debounce(func, wait) {
    let timeout;
    return function executedFunction(...args) {
        const later = () => {
            clearTimeout(timeout);
            func(...args);
        };
        clearTimeout(timeout);
        timeout = setTimeout(later, wait);
    };
}

// Optimized scroll listener
const optimizedScrollHandler = debounce(function() {
    // Your scroll handling logic here
}, 10);

window.addEventListener('scroll', optimizedScrollHandler);
```

## Quick Deployment Steps:

1. **Create Repository:**
   - Go to GitHub.com (logged in as solbanz352)
   - Click "New Repository"
   - Name: "sollaunch-platform"
   - Make it Public
   - Create Repository

2. **Upload Files:**
   - Copy each file content above into separate files
   - Upload to your GitHub repo
   - Commit with message: "Initial SolLaunch deployment"

3. **Deploy on Vercel:**
   - Go to vercel.com
   - Click "New Project"
   - Import from GitHub: solbanz352/sollaunch-platform
   - Click "Deploy"
   - Get your live URL!

The complete frontend package is now ready for deployment with all the enhancements: refined copy, 3D visuals, animations, SEO optimization, and mobile responsiveness.