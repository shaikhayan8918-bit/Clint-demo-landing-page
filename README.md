# Clint-demo-landing-page
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Free Asset Protection Blueprint - Anderson Business Advisors</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
            background-color: #f8f9fa;
        }

        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 0 20px;
        }

        .section {
            background: white;
            margin: 20px 0;
            padding: 40px 30px;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }

        .hero {
            background: linear-gradient(135deg, #1e3c72, #2a5298);
            color: white;
            text-align: center;
        }

        .preheader {
            background: #ff6b35;
            color: white;
            text-align: center;
            padding: 10px;
            font-weight: bold;
            font-size: 14px;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        h1 {
            font-size: 48px;
            font-weight: bold;
            margin: 20px 0;
            line-height: 1.2;
        }

        h2 {
            font-size: 32px;
            color: #1e3c72;
            margin: 30px 0 20px 0;
            font-weight: bold;
            text-align: center;
        }

        .subheader {
            font-size: 24px;
            margin: 20px 0 30px 0;
            font-weight: 300;
            line-height: 1.3;
        }

        .vsl-container {
            margin: 40px 0;
            text-align: center;
        }

        .vsl-icon {
            position: relative;
            display: inline-block;
            width: 300px;
            height: 200px;
            background: linear-gradient(45deg, #ff6b35, #f7931e);
            border-radius: 15px;
            cursor: pointer;
            transition: transform 0.3s ease;
            box-shadow: 0 8px 25px rgba(255, 107, 53, 0.3);
            text-decoration: none;
            color: white;
        }

        .vsl-icon:hover {
            transform: scale(1.05);
        }

        .play-button {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 70px;
            height: 70px;
            background: rgba(255,255,255,0.9);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .play-button::after {
            content: '';
            width: 0;
            height: 0;
            border-left: 20px solid #1e3c72;
            border-top: 12px solid transparent;
            border-bottom: 12px solid transparent;
            margin-left: 5px;
        }

        .vsl-text {
            position: absolute;
            bottom: 15px;
            left: 50%;
            transform: translateX(-50%);
            font-weight: bold;
            font-size: 16px;
            text-shadow: 0 2px 4px rgba(0,0,0,0.3);
        }

        .cta-button {
            background: linear-gradient(45deg, #28a745, #20c997);
            color: white;
            padding: 18px 40px;
            font-size: 20px;
            font-weight: bold;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            transition: all 0.3s ease;
            text-decoration: none;
            display: inline-block;
            margin: 20px 0;
            box-shadow: 0 4px 15px rgba(40, 167, 69, 0.4);
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .cta-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(40, 167, 69, 0.6);
        }

        p {
            font-size: 18px;
            margin: 15px 0;
            line-height: 1.8;
        }

        .highlight {
            background: #fff3cd;
            padding: 20px;
            border-left: 5px solid #ffc107;
            margin: 25px 0;
            border-radius: 5px;
        }

        .bullet-point {
            background: #e8f5e8;
            padding: 15px;
            margin: 15px 0;
            border-left: 4px solid #28a745;
            border-radius: 5px;
        }

        .value-stack {
            background: #f8f9fa;
            padding: 25px;
            border-radius: 10px;
            margin: 25px 0;
            border: 2px solid #dee2e6;
        }

        .price-highlight {
            font-size: 36px;
            color: #dc3545;
            text-decoration: line-through;
            display: inline-block;
            margin-right: 20px;
        }

        .free-price {
            font-size: 48px;
            color: #28a745;
            font-weight: bold;
        }

        .urgency-box {
            background: linear-gradient(45deg, #dc3545, #c82333);
            color: white;
            padding: 20px;
            border-radius: 10px;
            margin: 25px 0;
            text-align: center;
        }

        .form-container {
            background: #f8f9fa;
            padding: 30px;
            border-radius: 10px;
            margin: 25px 0;
            border: 2px solid #28a745;
        }

        .form-group {
            margin: 15px 0;
        }

        .form-group label {
            display: block;
            margin-bottom: 5px;
            font-weight: bold;
            color: #1e3c72;
        }

        .form-group input {
            width: 100%;
            padding: 12px;
            font-size: 16px;
            border: 2px solid #dee2e6;
            border-radius: 5px;
            transition: border-color 0.3s ease;
        }

        .form-group input:focus {
            outline: none;
            border-color: #28a745;
        }

        .checkbox-group {
            display: flex;
            align-items: flex-start;
            margin: 15px 0;
        }

        .checkbox-group input {
            width: auto;
            margin-right: 10px;
            margin-top: 5px;
        }

        .submit-btn {
            background: linear-gradient(45deg, #dc3545, #c82333);
            color: white;
            padding: 18px 50px;
            font-size: 22px;
            font-weight: bold;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            width: 100%;
            margin: 20px 0;
            transition: all 0.3s ease;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .submit-btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(220, 53, 69, 0.4);
        }

        .testimonial {
            background: #fff3cd;
            padding: 20px;
            border-radius: 10px;
            margin: 20px 0;
            font-style: italic;
            border-left: 5px solid #ffc107;
        }

        .faq-item {
            margin: 20px 0;
            padding: 20px;
            background: #f8f9fa;
            border-radius: 8px;
        }

        .faq-question {
            font-weight: bold;
            color: #1e3c72;
            font-size: 20px;
            margin-bottom: 10px;
        }

        .faq-answer {
            font-size: 16px;
            line-height: 1.6;
        }

        @media (max-width: 768px) {
            h1 { font-size: 36px; }
            h2 { font-size: 28px; }
            .subheader { font-size: 20px; }
            .container { padding: 0 15px; }
            .section { padding: 25px 20px; }
            .vsl-icon { width: 250px; height: 150px; }
            .cta-button { padding: 15px 30px; font-size: 18px; }
        }
    </style>
</head>
<body>
    <div class="preheader">
        ATTENTION: Real Estate Investors, Active Traders & Business Owners
    </div>

    <!-- HERO SECTION -->
    <div class="hero section">
        <div class="container">
            <h1>Get Your Custom Asset Protection Blueprint in Just 45 Minutes</h1>
            <div class="subheader">
                Shield your real estate and business investments from lawsuits... slash your tax burden by thousands... and build generational wealth — all WITHOUT dealing with confusing legal jargon or paying hourly attorney fees
            </div>
            
            <div class="vsl-container">
                <a href="https://docs.google.com/document/d/1g27qdnlMz5zfSKlp3rnrmhrbY0cB-f_u17joEwM-1eA/edit?usp=sharing" class="vsl-icon">
                    <div class="play-button"></div>
                    <div class="vsl-text">Click Here To See The: VSL I WROTE FOR YOU</div>
                </a>
            </div>

            <a href="#form" class="cta-button">CLAIM YOUR FREE BLUEPRINT NOW</a>
        </div>
    </div>

    <!-- PROBLEM IDENTIFICATION -->
    <div class="section">
        <div class="container">
            <h2>Why Most Real Estate Investors Wake Up at 3 AM Terrified</h2>
            
            <p>You've built something incredible.</p>
            
            <p>Maybe it's a portfolio of rental properties generating steady cash flow...</p>
            
            <p>Or a thriving business that's finally hitting those monthly revenue goals you dreamed about...</p>
            
            <p>But here's what keeps you staring at the ceiling at 3 AM:</p>
            
            <p><strong>One lawsuit. One angry tenant. One frivolous claim.</strong></p>
            
            <p>And everything you've worked for could vanish.</p>
            
            <div class="highlight">
                <p><strong>You've tried setting up an LLC through LegalZoom...</strong> Only to realize it offers about as much protection as a paper umbrella in a hurricane.</p>
                
                <p><strong>You've paid your local attorney $400/hour for "advice"...</strong> That left you more confused than when you started.</p>
                
                <p><strong>You've searched online for tax strategies...</strong> But found nothing that actually applies to your specific situation.</p>
            </div>
            
            <p>Meanwhile, you're watching <strong>40-50% of your hard-earned profits</strong> disappear to taxes every year...</p>
            
            <p>All because the "experts" gave you cookie-cutter solutions that don't actually work for real estate investors and business owners like you.</p>
            
            <p>But what if I told you there's a completely different approach?</p>
            
            <p>One that's already helped thousands of investors and entrepreneurs sleep peacefully... knowing their assets are bulletproof and their tax burden is slashed legally.</p>
        </div>
    </div>

    <!-- ORIGIN STORY -->
    <div class="section">
        <div class="container">
            <h2>The $847,000 Wake-Up Call That Changed Everything</h2>
            
            <p>Three years ago, I watched a successful real estate investor lose nearly everything.</p>
            
            <p>Sarah owned 12 rental properties across three states. She was pulling in $18,000 a month in passive income.</p>
            
            <p>She thought she was "protected" because she had an LLC...</p>
            
            <p>Until a tenant slipped on her property's front steps.</p>
            
            <p>The lawsuit didn't just target the property... it pierced through her flimsy LLC structure and went after her personal assets.</p>
            
            <p><strong>$847,000 later</strong>, Sarah lost 8 of her 12 properties.</p>
            
            <p>Why? Because she fell for the same myth that 90% of investors believe:</p>
            
            <div class="highlight">
                <p><strong>MYTH:</strong> "An LLC will protect me from everything."</p>
                <p><strong>REALITY:</strong> Most LLCs are set up wrong and offer zero real protection.</p>
            </div>
            
            <p>That's when I realized the entire system is broken.</p>
            
            <p>Traditional attorneys charge by the hour... so they have ZERO incentive to give you quick, actionable solutions.</p>
            
            <p>Generic online legal services treat your multi-million dollar portfolio like a $50 lawn mower.</p>
            
            <p>And CPAs? Most have never even owned a rental property, let alone understood the tax strategies that could save you tens of thousands.</p>
            
            <p>So we built something completely different...</p>
        </div>
    </div>

    <!-- SOLUTION REVELATION -->
    <div class="section">
        <div class="container">
            <h2>The "Fortress Strategy" That Shields Your Wealth From Every Angle</h2>
            
            <p>After studying how the ultra-wealthy protect their assets (and working with over 10,000+ real estate investors and business owners), we developed what we call the <strong>Fortress Strategy</strong>.</p>
            
            <p>Think of it like this...</p>
            
            <p>Most people build a house and put up a picket fence, thinking that's enough protection.</p>
            
            <p>The Fortress Strategy builds multiple walls, moats, and security systems around your wealth.</p>
            
            <div class="highlight">
                <p><strong>Layer 1:</strong> Properly structured entities that actually hold up in court</p>
                <p><strong>Layer 2:</strong> Advanced tax strategies that slash your burden legally</p>
                <p><strong>Layer 3:</strong> Estate planning that protects generational wealth</p>
                <p><strong>Layer 4:</strong> Ongoing professional support without hourly fees</p>
            </div>
            
            <p>Here's how it works:</p>
            
            <p><strong>First</strong>, we analyze your exact situation. Your properties, your business structure, your goals, your risk level.</p>
            
            <p><strong>Then</strong>, we design a custom blueprint that creates multiple layers of protection around your assets.</p>
            
            <p><strong>Finally</strong>, we show you exactly how to implement it without the confusion or massive legal bills.</p>
            
            <div class="bullet-point">
                <p><strong>Real Example:</strong> Marcus owned 6 rental properties and was paying $47,000 a year in unnecessary taxes. After implementing his custom blueprint, he now saves $31,000 annually — that's $310,000 over the next decade.</p>
            </div>
            
            <div class="bullet-point">
                <p><strong>Real Example:</strong> Jennifer's construction business was sued for $2.3 million. Because her entities were structured properly, the lawsuit couldn't touch her personal assets or other business ventures. She kept everything.</p>
            </div>
            
            <p>This isn't theoretical...</p>
            
            <p>It's a proven system that's already protected billions in investor wealth.</p>
        </div>
    </div>

    <!-- PRODUCT INTRODUCTION -->
    <div class="section">
        <div class="container">
            <h2>Introducing Your Personal 45-Minute Asset Protection Blueprint Session</h2>
            
            <p>For the first time ever, we're offering our complete asset protection assessment — the same one our high-net-worth clients pay $750 for — completely free.</p>
            
            <p>Here's exactly what happens in your session:</p>
            
            <div class="bullet-point">
                <p><strong>Liability Risk Assessment:</strong> We identify every vulnerability in your current structure that could cost you everything → You'll know exactly where you're exposed and how to fix it → You'll sleep peacefully knowing your wealth is truly protected</p>
            </div>
            
            <div class="bullet-point">
                <p><strong>Custom Entity Blueprint:</strong> We design the optimal structure for YOUR specific situation → No more generic advice that doesn't apply to you → You'll have a clear roadmap for bulletproof asset protection</p>
            </div>
            
            <div class="bullet-point">
                <p><strong>Tax Minimization Strategy:</strong> We reveal legal strategies to slash your tax burden → Stop overpaying Uncle Sam by thousands every year → Keep more of what you earn to reinvest and grow</p>
            </div>
            
            <div class="bullet-point">
                <p><strong>Estate Planning Foundation:</strong> We outline how to pass wealth to your heirs efficiently → Avoid probate nightmares and estate taxes → Build a lasting legacy for your family</p>
            </div>
            
            <p>Unlike those hour-long sales pitches disguised as "consultations," this is a real working session.</p>
            
            <p>You'll walk away with specific, actionable strategies you can implement immediately.</p>
            
            <p>No fluff. No filler. Just pure value.</p>
        </div>
    </div>

    <!-- OFFER STRUCTURE -->
    <div class="section">
        <div class="container">
            <h2>What You Get in Your Free Strategy Session</h2>
            
            <div class="value-stack">
                <p><strong>✓ Personal Asset Protection Assessment</strong></p>
                <p>Normally $200 - Identify every vulnerability in your current setup</p>
                <br>
                <p><strong>✓ Custom Entity Structure Design</strong></p>
                <p>Normally $300 - Blueprints for optimal protection and tax savings</p>
                <br>
                <p><strong>✓ Tax Strategy Consultation</strong></p>
                <p>Normally $150 - Legal ways to minimize your tax burden</p>
                <br>
                <p><strong>✓ Estate Planning Overview</strong></p>
                <p>Normally $100 - Foundation for generational wealth transfer</p>
                <br>
                <p style="border-top: 2px solid #333; padding-top: 15px; font-weight: bold; font-size: 20px;">
                    Total Value: <span class="price-highlight">$750</span>
                </p>
            </div>
            
            <div style="text-align: center; margin: 30px 0;">
                <p style="font-size: 24px; margin-bottom: 10px;">Your Investment Today:</p>
                <div class="free-price">FREE</div>
                <p style="font-size: 18px; color: #666; margin-top: 10px;">U.S. Residents Only</p>
            </div>
            
            <div class="highlight">
                <p><strong>100% Risk-Free Guarantee:</strong> If you don't walk away with at least one strategy that could save you thousands in taxes or protect your assets better, we'll personally refund the time you spent with us by sending you a $50 Amazon gift card.</p>
            </div>
            
            <div class="urgency-box">
                <p style="font-size: 22px; font-weight: bold;">⚠️ LIMITED AVAILABILITY WARNING ⚠️</p>
                <p>We can only handle 47 new strategy sessions this month due to the personalized nature of each consultation. Once those spots are filled, the next available appointment won't be until next month.</p>
                <p style="margin-top: 15px; font-size: 18px;">Book yours now before they're gone.</p>
            </div>
            
            <div style="text-align: center;">
                <a href="#form" class="cta-button">SECURE MY FREE BLUEPRINT SESSION</a>
            </div>
        </div>
    </div>

    <!-- FORM SECTION -->
    <div class="section" id="form">
        <div class="container">
            <h2>Get Your Free Asset Protection Blueprint</h2>
            
            <div class="form-container">
                <form action="#" method="POST">
                    <div class="form-group">
                        <label for="firstName">First Name</label>
                        <input type="text" id="firstName" name="firstName" required>
                    </div>
                    
                    <div class="form-group">
                        <label for="lastName">Last Name</label>
                        <input type="text" id="lastName" name="lastName" required>
                    </div>
                    
                    <div class="form-group">
                        <label for="email">Email Address</label>
                        <input type="email" id="email" name="email" required>
                    </div>
                    
                    <div class="form-group">
                        <label for="phone">Mobile Phone</label>
                        <input type="tel" id="phone" name="phone" required>
                    </div>
                    
                    <div class="form-group">
                        <label for="zipCode">ZIP Code</label>
                        <input type="text" id="zipCode" name="zipCode" required>
                    </div>
                    
                    <div class="checkbox-group">
                        <input type="checkbox" id="smsConsent" name="smsConsent" required>
                        <label for="smsConsent">I consent to receive SMS reminders about my strategy session appointment.</label>
                    </div>
                    
                    <button type="submit" class="submit-btn">BOOK MY FREE SESSION NOW</button>
                    
                    <p style="font-size: 14px; color: #666; text-align: center; margin-top: 15px;">
                        U.S. residents only. By submitting this form, you agree to receive communications from Anderson Business Advisors.
                    </p>
                </form>
            </div>
        </div>
    </div>

    <!-- FAQ SECTION -->
    <div class="section">
        <div class="container">
            <h2>Your Most Important Questions Answered</h2>
            
            <div class="faq-item">
                <div class="faq-question">Is this really free, or will you try to sell me something?</div>
                <div class="faq-answer">The 45-minute strategy session is completely free with zero obligations. Yes, we may mention our ongoing services if they're a perfect fit for your situation, but there's no pressure whatsoever. Many clients get tremendous value from the free session alone.</div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">I already have an LLC. Do I still need this?</div>
                <div class="faq-answer">Absolutely. Most LLCs are set up incorrectly and offer minimal protection. We'll review your current structure and show you exactly what's missing. You might be one simple adjustment away from bulletproof protection.</div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">What if I only have one rental property?</div>
                <div class="faq-answer">Perfect! It's much easier (and cheaper) to set up proper protection from the beginning than to fix problems later. Whether you have 1 property or 100, you need the same level of protection.</div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">How is this different from my CPA or attorney?</div>
                <div class="faq-answer">Most CPAs and attorneys work in silos — your CPA handles taxes, your attorney handles legal, but nobody coordinates the strategy. We integrate everything: tax planning, asset protection, and estate planning work together as one cohesive system.</div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">What happens after the strategy session?</div>
                <div class="faq-answer">You'll have a clear blueprint you can implement yourself, or we can handle everything for you through our ongoing services. The choice is entirely yours — there's no pressure either way.</div>
            </div>
            
            <div style="text-align: center; margin-top: 40px;">
                <p style="font-size: 20px; margin-bottom: 20px;">Ready to protect what you've built?</p>
                <a href="#form" class="cta-button">CLAIM YOUR FREE BLUEPRINT NOW</a>
            </div>
        </div>
    </div>
</body>
</html>
