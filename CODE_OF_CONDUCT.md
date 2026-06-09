<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Nexvoya Logistics — Global Shipment &amp; Commerce Platform</title>
<link href="https://fonts.googleapis.com/css2?family=Syne:wght@400;600;700;800&family=Inter:wght@300;400;500;600&family=JetBrains+Mono:wght@400;500&display=swap" rel="stylesheet">
<style>
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
:root{
  --navy:#0A0F1E;--steel:#0E1525;--panel:#111827;--card:#141E33;--card2:#1A2540;
  --border:#1E2D4A;--border2:#243558;
  --teal:#00D4B8;--teal2:#00A896;--teal-glow:rgba(0,212,184,.12);
  --amber:#F59E0B;--red:#EF4444;--green:#10B981;--purple:#8B5CF6;--blue:#3B82F6;
  --gold:#FFD700;
  --slate:#94A3B8;--light:#CBD5E1;--white:#F8FAFC;
  --ff-disp:'Syne',sans-serif;--ff-body:'Inter',sans-serif;--ff-mono:'JetBrains Mono',monospace;
}
html{scroll-behavior:smooth}
body{background:var(--navy);color:var(--light);font-family:var(--ff-body);font-size:14px;line-height:1.6;overflow-x:hidden}

/* ═══ SCROLLBAR ═══ */
::-webkit-scrollbar{width:5px}
::-webkit-scrollbar-track{background:var(--navy)}
::-webkit-scrollbar-thumb{background:var(--border2);border-radius:3px}

/* ═══ NAV ═══ */
nav{
  position:fixed;top:0;left:0;right:0;z-index:200;
  display:flex;align-items:center;justify-content:space-between;
  padding:0 40px;height:62px;
  background:rgba(10,15,30,.92);backdrop-filter:blur(16px);
  border-bottom:1px solid var(--border);
}
.nav-logo{display:flex;align-items:center;gap:10px;font-family:var(--ff-disp);font-size:19px;font-weight:800;color:var(--white);letter-spacing:-.3px;cursor:pointer}
.nav-logo-icon{width:32px;height:32px;background:var(--teal);border-radius:8px;display:flex;align-items:center;justify-content:center;font-size:15px}
.nav-logo span{color:var(--teal)}
.nav-links{display:flex;align-items:center;gap:6px}
.nav-links a{color:var(--slate);text-decoration:none;font-size:13px;padding:6px 12px;border-radius:6px;transition:all .2s;white-space:nowrap}
.nav-links a:hover{color:var(--white);background:rgba(255,255,255,.05)}
.nav-live{display:flex;align-items:center;gap:6px;background:rgba(0,212,184,.1);border:1px solid rgba(0,212,184,.25);color:var(--teal);padding:5px 12px;border-radius:20px;font-size:12px;font-weight:500}
.pdot{width:6px;height:6px;border-radius:50%;background:var(--teal);animation:pulse 2s infinite}
@keyframes pulse{0%,100%{opacity:1;transform:scale(1)}50%{opacity:.4;transform:scale(1.6)}}

/* ═══ HERO ═══ */
.hero{
  padding-top:62px;min-height:100vh;
  display:grid;grid-template-columns:1fr 1fr;
  background:radial-gradient(ellipse 80% 60% at 70% 40%,rgba(0,212,184,.06) 0%,transparent 60%);
  position:relative;overflow:hidden;
}
.hero::before{
  content:'';position:absolute;inset:0;
  background:url("data:image/svg+xml,%3Csvg width='60' height='60' xmlns='http://www.w3.org/2000/svg'%3E%3Cdefs%3E%3Cpattern id='g' width='60' height='60' patternUnits='userSpaceOnUse'%3E%3Ccircle cx='30' cy='30' r='.6' fill='%2300D4B8' opacity='.12'/%3E%3C/pattern%3E%3C/defs%3E%3Crect width='100%25' height='100%25' fill='url(%23g)'/%3E%3C/svg%3E");
  pointer-events:none;
}
.hero-left{display:flex;flex-direction:column;justify-content:center;padding:80px 48px;position:relative;z-index:1}
.eyebrow{display:inline-flex;align-items:center;gap:8px;font-family:var(--ff-mono);font-size:11px;font-weight:500;color:var(--teal);letter-spacing:2px;text-transform:uppercase;margin-bottom:22px}
.eyebrow::before{content:'';display:block;width:24px;height:1px;background:var(--teal)}
h1{font-family:var(--ff-disp);font-size:clamp(34px,4vw,58px);font-weight:800;line-height:1.06;letter-spacing:-1.5px;color:var(--white);margin-bottom:22px}
h1 em{font-style:normal;color:var(--teal)}
.hero-sub{font-size:16px;color:var(--slate);max-width:460px;line-height:1.75;margin-bottom:36px}
.hero-btns{display:flex;gap:12px;flex-wrap:wrap}
.btn-p{background:var(--teal);color:var(--navy);padding:13px 26px;border-radius:8px;font-size:14px;font-weight:700;border:none;cursor:pointer;transition:all .2s;text-decoration:none;display:inline-flex;align-items:center;gap:8px}
.btn-p:hover{background:#00bda6;transform:translateY(-1px);box-shadow:0 8px 24px rgba(0,212,184,.25)}
.btn-o{background:transparent;color:var(--white);padding:12px 26px;border-radius:8px;font-size:14px;font-weight:500;border:1px solid var(--border2);cursor:pointer;transition:all .2s;text-decoration:none;display:inline-flex;align-items:center;gap:8px}
.btn-o:hover{border-color:var(--teal);color:var(--teal)}
.hero-stats{display:flex;gap:40px;margin-top:52px;padding-top:36px;border-top:1px solid var(--border)}
.hs-val">142<span>K</span></div><div class="hs-lbl">Active shipments</div></div>
      <div><div class="hs-val">98.<span>4%</span></div><div class="hs-lbl">On-time rate</div></div>
      <div><div class="hs-val">18</div><div class="hs-lbl">Service levels</div></div>
      <div><div class="hs-val">4</div><div class="hs-lbl">Payment methods</div></div>
    </div>
  </div>
  <div class="hero-right">
    <div style="position:relative">
      <canvas id="globe" width="680" height="680"></canvas>
      <div class="rb">
        <div class="rb-dot" style="background:#00D4B8"></div>
        <div><div class="rb-r">SHA → LAX</div><div class="rb-s">In transit · 4d 12h</div></div>
      </div>
      <div class="rb">
        <div class="rb-dot" style="background:#F59E0B"></div>
        <div><div class="rb-r">DXB → LHR</div><div class="rb-s">Customs · 6h ETA</div></div>
      </div>
      <div class="rb">
        <div class="rb-dot" style="background:#10B981"></div>
        <div><div class="rb-r">NYC → CDG</div><div class="rb-s">Delivered ✓</div></div>
      </div>
    </div>
  </div>
</section>

<section class="sec bg-steel" id="store">
  <div class="sec-hdr">
    <div>
      <div class="sec-ey">Nexvoya Marketplace</div>
      <h2>Store — Goods, Services &amp; Digital Assets</h2>
    </div>
    <a href="#" class="sec-act">Browse all listings ↗</a>
  </div>

  <div class="store-tabs">
    <div class="stab active" onclick="filterStore('all',this)">All Products</div>
    <div class="stab" onclick="filterStore('goods',this)">📦 Physical Goods</div>
    <div class="stab" onclick="filterStore('services',this)">🛠 Services</div>
    <div class="stab" onclick="filterStore('digital',this)">💎 Digital Assets</div>
    <div class="stab" onclick="filterStore('bookings',this)">📅 Bookings</div>
  </div>

  <div class="prod-grid" id="prodGrid">
    <div class="prod-card" data-cat="goods">
      <div class="prod-thumb" style="background:linear-gradient(135deg,#0e2040,#142a50)">🚢<div class="prod-badge badge-new">NEW</div></div>
      <div class="prod-body">
        <div class="prod-cat">Physical Goods</div>
        <div class="prod-name">Industrial Freight Container — 20ft</div>
        <div class="prod-desc">ISO-certified, weatherproof steel container ready for full container load (FCL) ocean shipments.</div>
        <div class="prod-foot"><div class="prod-price">$4,888 <small>/unit</small></div><button class="add-btn">Add to Cart</button></div>
      </div>
    </div>

    <div class="prod-card" data-cat="goods">
      <div class="prod-thumb" style="background:linear-gradient(135deg,#1a1030,#26184a)">📦<div class="prod-badge badge-hot">HOT</div></div>
      <div class="prod-body">
        <div class="prod-cat">Physical Goods</div>
        <div class="prod-name">Cold-Chain Pallet Liner Kit (50-pack)</div>
        <div class="prod-desc">Multi-layer insulated pallet liners for pharmaceutical and perishable cargo. Temp-rated −20°C to +25°C.</div>
        <div class="prod-foot"><div class="prod-price">$1,288 <small>/carton</small></div><button class="add-btn">Add to Cart</button></div>
      </div>
    </div>

    <div class="prod-card" data-cat="goods">
      <div class="prod-thumb" style="background:linear-gradient(135deg,#0e2030,#102840)">🏷️<div class="prod-badge badge-new">NEW</div></div>
      <div class="prod-body">
        <div class="prod-cat">Physical Goods</div>
        <div class="prod-name">Smart IoT Cargo Tracker — GPS+BLE</div>
        <div class="prod-desc">Rugged tracker with real-time GPS, humidity, shock & temperature sensors. 12-month battery life.</div>
        <div class="prod-foot"><div class="prod-price">$488 <small>/device</small></div><button class="add-btn">Add to Cart</button></div>
      </div>
    </div>

    <div class="prod-card" data-cat="goods">
      <div class="prod-thumb" style="background:linear-gradient(135deg,#0d1a35,#152240)">⚡<div class="prod-badge badge-hot">HOT</div></div>
      <div class="prod-body">
        <div class="prod-cat">Physical Goods</div>
        <div class="prod-name">Hazmat Certified Packaging Set</div>
        <div class="prod-desc">UN-rated dangerous goods packaging. IATA/IMDG compliant. For air &amp; sea regulated cargo.</div>
        <div class="prod-foot"><div class="prod-price">$288 <small>/set</small></div><button class="add-btn">Add to Cart</button></div>
      </div>
    </div>

    <div class="prod-card" data-cat="services">
      <div class="prod-thumb" style="background:linear-gradient(135deg,#0e2038,#0c2030)">🛃<div class="prod-badge badge-new">NEW</div></div>
      <div class="prod-body">
        <div class="prod-cat">Services</div>
        <div class="prod-name">Customs Brokerage &amp; Clearance</div>
        <div class="prod-desc">End-to-end import/export documentation, tariff classification, and customs clearance in 140+ countries.</div>
        <div class="prod-foot"><div class="prod-price">$588 <small>/shipment</small></div><button class="add-btn">Book Now</button></div>
      </div>
    </div>

    <div class="prod-card" data-cat="services">
      <div class="prod-thumb" style="background:linear-gradient(135deg,#0d1d38,#0f2040)">📋<div class="prod-badge badge-hot">HOT</div></div>
      <div class="prod-body">
        <div class="prod-cat">Services</div>
        <div class="prod-name">Supply Chain Audit &amp; Consulting</div>
        <div class="prod-desc">Expert 30-day audit of your freight flows, cost structure, and vendor contracts with optimisation report.</div>
        <div class="prod-foot"><div class="prod-price">$3,888 <small>/engagement</small></div><button class="add-btn">Book Now</button></div>
      </div>
    </div>

    <div class="prod-card" data-cat="services">
      <div class="prod-thumb" style="background:linear-gradient(135deg,#0a1830,#0d2038)">🏗️</div>
      <div class="prod-body">
        <div class="prod-cat">Services</div>
        <div class="prod-name">Bonded Warehouse — Monthly Lease</div>
        <div class="prod-desc">Secure, climate-controlled bonded warehouse space in Rotterdam, Singapore, or Dubai. Minimum 1 month.</div>
        <div class="prod-foot"><div class="prod-price">$988 <small>/mo</small></div><button class="add-btn">Reserve Space</button></div>
      </div>
    </div>

    <div class="prod-card" data-cat="services">
      <div class="prod-thumb" style="background:linear-gradient(135deg,#0e2038,#0a1a30)">🚛</div>
      <div class="prod-body">
        <div class="prod-cat">Services</div>
        <div class="prod-name">Last-Mile Delivery Network Access</div>
        <div class="prod-desc">API access to 80+ last-mile carrier integrations. Automated label generation, tracking, and returns.</div>
        <div class="prod-foot"><div class="prod-price">$188 <small>/mo</small></div><button class="add-btn">Activate</button></div>
      </div>
    </div>

    <div class="prod-card" data-cat="digital">
      <div class="prod-thumb" style="background:linear-gradient(135deg,#1a0a3a,#2a1050)">💎<div class="prod-badge badge-dig">DIGITAL</div></div>
      <div class="prod-body">
        <div class="prod-cat">Digital Asset</div>
        <div class="prod-name">NVX Route Token — APAC Corridor</div>
        <div class="prod-desc">Tokenized freight capacity on the Asia-Pacific corridor. Redeemable for discounted container bookings.</div>
        <div class="prod-foot"><div class="prod-price">$888 <small>/token</small></div><button class="add-btn">Buy Token</button></div>
      </div>
    </div>

    <div class="prod-card" data-cat="digital">
      <div class="prod-thumb" style="background:linear-gradient(135deg,#1a0830,#260c48)">🔑<div class="prod-badge badge-dig">DIGITAL</div></div>
      <div class="prod-body">
        <div class="prod-cat">Digital Asset</div>
        <div class="prod-name">Smart Contract — Trade Finance Module</div>
        <div class="prod-desc">Automated on-chain letter of credit and invoice financing smart contract, pre-audited by CertiK.</div>
        <div class="prod-foot"><div class="prod-price">$2,888 <small>/license</small></div><button class="add-btn">License</button></div>
      </div>
    </div>

    <div class="prod-card" data-cat="digital">
      <div class="prod-thumb" style="background:linear-gradient(135deg,#0e1040,#141858)">📊<div class="prod-badge badge-dig">DIGITAL</div></div>
      <div class="prod-body">
        <div class="prod-cat">Digital Asset</div>
        <div class="prod-name">Logistics Intelligence Data API</div>
        <div class="prod-desc">Real-time port congestion, rate benchmarks, and vessel AIS data feed. JSON/GraphQL. 99.9% SLA.</div>
        <div class="prod-foot"><div class="prod-price">$488 <small>/mo</small></div><button class="add-btn">Subscribe</button></div>
      </div>
    </div>

    <div class="prod-card" data-cat="digital">
      <div class="prod-thumb" style="background:linear-gradient(135deg,#1a1030,#241440)">🎫<div class="prod-badge badge-dig">DIGITAL</div></div>
      <div class="prod-body">
        <div class="prod-cat">Digital Asset</div>
        <div class="prod-name">Nexvoya Pro Dashboard License</div>
        <div class="prod-desc">Unlimited team seats, white-label portal, advanced analytics, and priority API rate limits. Annual license.</div>
        <div class="prod-foot"><div class="prod-price">$1,888 <small>/yr</small></div><button class="add-btn">Get License</button></div>
      </div>
    </div>

    <div class="prod-card" data-cat="bookings">
      <div class="prod-thumb" style="background:linear-gradient(135deg,#0e2830,#102e38)">🛳️<div class="prod-badge badge-bk">BOOKING</div></div>
      <div class="prod-body">
        <div class="prod-cat">Booking</div>
        <div class="prod-name">Full Container Load (FCL) — Ocean</div>
        <div class="prod-desc">Book 20ft or 40ft FCL slots on major ocean lanes. Shanghai, Rotterdam, Singapore origin ports.</div>
        <div class="prod-foot"><div class="prod-price">$2,188 <small>/slot</small></div><button class="add-btn">Book Slot</button></div>
      </div>
    </div>

    <div class="prod-card" data-cat="bookings">
      <div class="prod-thumb" style="background:linear-gradient(135deg,#0a1e2a,#0e2838)">✈️<div class="prod-badge badge-bk">BOOKING</div></div>
      <div class="prod-body">
        <div class="prod-cat">Booking</div>
        <div class="prod-name">Air Freight Priority Slot</div>
        <div class="prod-desc">Guaranteed next-flight priority air cargo slot on trans-Pacific and Europe-Asia lanes. 100kg minimum.</div>
        <div class="prod-foot"><div class="prod-price">$1,488 <small>/slot</small></div><button class="add-btn">Book Slot</button></div>
      </div>
    </div>

    <div class="prod-card" data-cat="bookings">
      <div class="prod-thumb" style="background:linear-gradient(135deg,#0c1e30,#102230)">🏬<div class="prod-badge badge-bk">BOOKING</div></div>
      <div class="prod-body">
        <div class="prod-cat">Booking</div>
        <div class="prod-name">Port Inspection &amp; Survey Service</div>
        <div class="prod-desc">On-site cargo condition inspection at any of our 140 port nodes. Certified surveyors, same-day report.</div>
        <div class="prod-foot"><div class="prod-price">$388 <small>/inspection</small></div><button class="add-btn">Book Now</button></div>
      </div>
    </div>

    <div class="prod-card" data-cat="bookings">
      <div class="prod-thumb" style="background:linear-gradient(135deg,#0e2030,#102438)">🤝<div class="prod-badge badge-bk">BOOKING</div></div>
      <div class="prod-body">
        <div class="prod-cat">Booking</div>
        <div class="prod-name">1-on-1 Freight Strategy Session</div>
        <div class="prod-desc">60-minute consultation with a senior Nexvoya logistics specialist. Route optimisation &amp; carrier selection.</div>
        <div class="prod-foot"><div class="prod-price">$188 <small>/session</small></div><button class="add-btn">Book Session</button></div>
      </div>
    </div>
  </div>
</section>

<section class="sec bg-panel" id="staking-yields">
  <div class="sec-hdr">
    <div>
      <div class="sec-ey">Institutional Wealth Desk</div>
      <h2>Digital Asset Staking &amp; Capital Allocation</h2>
    </div>
    <div class="sec-act" style="color:var(--green)">Constant Verified Returns ✓</div>
  </div>

  <div class="dash-container">
    <div class="dash-panel">
      <div class="dash-title">📁 Project Operating Sectors</div>
      <div class="dash-selector" id="projectSelector">
        <div class="asset-item active" onclick="selectProject(0, this)">
          <div class="asset-meta">
            <div class="asset-icon">🛡️</div>
            <div>
              <div class="asset-sector">Cybersecurity &amp; Threat Intel</div>
              <div class="asset-title">Sentinel Shield Node (SSN)</div>
            </div>
          </div>
          <div class="asset-yields">
            <div class="yield-badge">+6.2%</div>
            <div class="yield-term">Short-Term Base</div>
          </div>
        </div>
        <div class="asset-item" onclick="selectProject(1, this)">
          <div class="asset-meta">
            <div class="asset-icon">🌐</div>
            <div>
              <div class="asset-sector">Decentralized Infra (DePIN)</div>
              <div class="asset-title">Nexus Core Corridor Ledger</div>
            </div>
          </div>
          <div class="asset-yields">
            <div class="yield-badge">+7.5%</div>
            <div class="yield-term">Short-Term Base</div>
          </div>
        </div>
        <div class="asset-item" onclick="selectProject(2, this)">
          <div class="asset-meta">
            <div class="asset-icon">🚢</div>
            <div>
              <div class="asset-sector">Tokenized Commodities</div>
              <div class="asset-title">Global Freight Liquidity Pool</div>
            </div>
          </div>
          <div class="asset-yields">
            <div class="yield-badge">+5.8%</div>
            <div class="yield-term">Short-Term Base</div>
          </div>
        </div>
        <div class="asset-item" onclick="selectProject(3, this)">
          <div class="asset-meta">
            <div class="asset-icon">🏦</div>
            <div>
              <div class="asset-sector">On-Chain Trade Finance</div>
              <div class="asset-title">RWA Autonomous Letter of Credit</div>
            </div>
          </div>
          <div class="asset-yields">
            <div class="yield-badge">+8.1%</div>
            <div class="yield-term">Short-Term Base</div>
          </div>
        </div>
      </div>
    </div>

    <div class="invest-workspace">
      <div>
        <div class="workspace-header">
          <div>
            <div class="active-project-name" id="wkName">Sentinel Shield Node (SSN)</div>
            <div class="active-project-sector" id="wkSector">Cybersecurity &amp; Threat Intel</div>
          </div>
          <div style="text-align: right">
            <div class="sec-ey" style="margin-bottom: 0;">Risk Rating</div>
            <div style="font-family: var(--ff-mono); font-size:12px; color: var(--green); font-weight:700;">PRO-GRADE AAA</div>
          </div>
        </div>

        <div class="term-toggle">
          <div class="term-btn active" id="btnShort" onclick="setTerm('short')">Short-Term (30-90 Day Lock)</div>
          <div class="term-btn" id="btnLong" onclick="setTerm('long')">Long-Term (180-365 Day Compound)</div>
        </div>

        <div class="level-slider-container">
          <div class="calc-label" style="display:flex; justify-content:space-between;">
            <span>Select Investment Tier Matrix</span>
            <span id="currentLevelDisplay" style="color:var(--teal); font-weight:700;">LEVEL 1</span>
          </div>
          <input type="range" min="1" max="8" value="1" class="level-slider" id="levelSlider" oninput="updateSliderMetrics()">
          <div class="level-indicator-bar">
            <span class="lvl-dot-label active" onclick="setSliderValue(1)">L1</span>
            <span class="lvl-dot-label" onclick="setSliderValue(2)">L2</span>
            <span class="lvl-dot-label" onclick="setSliderValue(3)">L3</span>
            <span class="lvl-dot-label" onclick="setSliderValue(4)">L4</span>
            <span class="lvl-dot-label" onclick="setSliderValue(5)">L5</span>
            <span class="lvl-dot-label" onclick="setSliderValue(6)">L6</span>
            <span class="lvl-dot-label" onclick="setSliderValue(7)">L7</span>
            <span class="lvl-dot-label" onclick="setSliderValue(8)">L8</span>
          </div>
        </div>

        <div class="calc-label">Enter Stake Principal Amount</div>
        <div class="calc-input-wrapper">
          <input type="number" class="calc-input" id="principalInput" value="88.98" min="88.98" max="100000" step="0.01" oninput="calculateReturns()">
          <span class="input-hint">USD VALUE ($88.98 - $100K Max)</span>
        </div>
      </div>

      <div>
        <div class="calc-grid">
          <div class="calc-box">
            <div class="calc-label">Constant Yield Rate</div>
            <div class="calc-value" id="calcRate" style="color:var(--green)">6.20%</div>
          </div>
          <div class="calc-box">
            <div class="calc-label">Projected Net Returns</div>
            <div class="calc-value" id="calcReturns" style="color:var(--teal)">$5.52</div>
          </div>
        </div>
        <button class="btn-invest" onclick="alert('Securing connection context... Forwarding allocation setup details to payment desk below.')">
          Execute Asset Allocation Securely →
        </button>
      </div>
    </div>
  </div>
</section>

<section class="sec bg-navy" id="pricing">
  <div class="sec-hdr">
    <div>
      <div class="sec-ey">Service Tiers</div>
      <h2>18 Pricing Levels — Starting at $19.88</h2>
    </div>
    <a href="#payments" class="sec-act">Choose a plan →</a>
  </div>

  <div class="pricing-wrap">
    <div class="pricing-track" id="pricingTrack">
      <div class="price-lvl">
        <div class="lvl-num">LEVEL 01</div>
        <div class="lvl-name">Starter Access</div>
        <div class="lvl-price">$19.88 <span>/mo</span></div>
        <ul class="lvl-features">
          <li>1 shipment/month</li>
          <li>Basic tracking dashboard</li>
          <li>Email support</li>
        </ul>
        <button class="lvl-btn">Select</button>
      </div>

      <div class="price-lvl">
        <div class="lvl-num">LEVEL 02</div>
        <div class="lvl-name">Explorer</div>
        <div class="lvl-price">$49.88 <span>/mo</span></div>
        <ul class="lvl-features">
          <li>5 shipments/month</li>
          <li>Live tracking + alerts</li>
          <li>1 API key</li>
        </ul>
        <button class="lvl-btn">Select</button>
      </div>

      <div class="price-lvl">
        <div class="lvl-num">LEVEL 03</div>
        <div class="lvl-name">Navigator</div>
        <div class="lvl-price">$99.88 <span>/mo</span></div>
        <ul class="lvl-features">
          <li>15 shipments/month</li>
          <li>Route optimiser</li>
          <li>3 API keys</li>
        </ul>
        <button class="lvl-btn">Select</button>
      </div>

      <div class="price-lvl">
        <div class="lvl-num">LEVEL 04</div>
        <div class="lvl-name">Voyager</div>
        <div class="lvl-price">$199.88 <span>/mo</span></div>
        <ul class="lvl-features">
          <li>40 shipments/month</li>
          <li>Customs doc automation</li>
          <li>5 API keys</li>
        </ul>
        <button class="lvl-btn">Select</button>
      </div>

      <div class="price-lvl featured">
        <div class="lvl-num">LEVEL 05</div>
        <div class="lvl-name">Commerce Pro</div>
        <div class="lvl-price">$399.88 <span>/mo</span></div>
        <ul class="lvl-features">
          <li>100 shipments/month</li>
          <li>Token wallet included</li>
          <li>Dedicated account rep</li>
        </ul>
        <button class="lvl-btn">Select</button>
      </div>

      <div class="price-lvl">
        <div class="lvl-num">LEVEL 06</div>
        <div class="lvl-name">Trade Pulse</div>
        <div class="lvl-price">$699.88 <span>/mo</span></div>
        <ul class="lvl-features">
          <li>200 shipments/month</li>
          <li>Advanced analytics suite</li>
          <li>Crypto payment enabled</li>
        </ul>
        <button class="lvl-btn">Select</button>
      </div>

      <div class="price-lvl">
        <div class="lvl-num">LEVEL 07</div>
        <div class="lvl-name">Freight Hub</div>
        <div class="lvl-price">$988.88 <span>/mo</span></div>
        <ul class="lvl-features">
          <li>350 shipments/month</li>
          <li>Multi-modal booking</li>
          <li>Cold chain tracking</li>
        </ul>
        <button class="lvl-btn">Select</button>
      </div>

      <div class="price-lvl">
        <div class="lvl-num">LEVEL 08</div>
        <div class="lvl-name">Supply Chain+</div>
        <div class="lvl-price">$1,488.88 <span>/mo</span></div>
        <ul class="lvl-features">
          <li>600 shipments/month</li>
          <li>Bonded WH access</li>
          <li>White-label portal</li>
        </ul>
        <button class="lvl-btn">Select</button>
      </div>

      <div class="price-lvl">
        <div class="lvl-num">LEVEL 09</div>
        <div class="lvl-name">Node Partner</div>
        <div class="lvl-price">$1,988.88 <span>/mo</span></div>
        <ul class="lvl-features">
          <li>1,000 shipments/month</li>
          <li>Node co-location access</li>
          <li>Trade finance tools</li>
        </ul>
        <button class="lvl-btn">Select</button>
      </div>

      <div class="price-lvl">
        <div class="lvl-num">LEVEL 10</div>
        <div class="lvl-name">Global Operator</div>
        <div class="lvl-price">$2,988.88 <span>/mo</span></div>
        <ul class="lvl-features">
          <li>2,000 shipments/month</li>
          <li>5 regional nodes</li>
          <li>Smart contract module</li>
        </ul>
        <button class="lvl-btn">Select</button>
      </div>

      <div class="price-lvl">
        <div class="lvl-num">LEVEL 11</div>
        <div class="lvl-name">Market Maker</div>
        <div class="lvl-price">$4,188.88 <span>/mo</span></div>
        <ul class="lvl-features">
          <li>3,500 shipments/month</li>
          <li>Digital asset vault</li>
          <li>ESG reporting suite</li>
        </ul>
        <button class="lvl-btn">Select</button>
      </div>

      <div class="price-lvl">
        <div class="lvl-num">LEVEL 12</div>
        <div class="lvl-name">Corridor Elite</div>
        <div class="lvl-price">$5,988.88 <span>/mo</span></div>
        <ul class="lvl-features">
          <li>5,000 shipments/month</li>
          <li>Dedicated port liaison</li>
          <li>Air express priority</li>
        </ul>
        <button class="lvl-btn">Select</button>
      </div>

      <div class="price-lvl">
        <div class="lvl-num">LEVEL 13</div>
        <div class="lvl-name">Enterprise Bridge</div>
        <div class="lvl-price">$7,988.88 <span>/mo</span></div>
        <ul class="lvl-features">
          <li>8,000 shipments/month</li>
          <li>ERP integration support</li>
          <li>Regulatory compliance desk</li>
        </ul>
        <button class="lvl-btn">Select</button>
      </div>

      <div class="price-lvl">
        <div class="lvl-num">LEVEL 14</div>
        <div class="lvl-name">Institutional</div>
        <div class="lvl-price">$11,988.88 <span>/mo</span></div>
        <ul class="lvl-features">
          <li>12,000 shipments/month</li>
          <li>Multi-entity management</li>
          <li>Private node deployment</li>
        </ul>
        <button class="lvl-btn">Select</button>
      </div>

      <div class="price-lvl">
        <div class="lvl-num">LEVEL 15</div>
        <div class="lvl-name">Sovereign Fleet</div>
        <div class="lvl-price">$18,888.88 <span>/mo</span></div>
        <ul class="lvl-features">
          <li>20,000 shipments/month</li>
          <li>Fleet tracking suite</li>
          <li>Sovereign data residency</li>
        </ul>
        <button class="lvl-btn">Select</button>
      </div>

      <div class="price-lvl">
        <div class="lvl-num">LEVEL 16</div>
        <div class="lvl-name">Continental</div>
        <div class="lvl-price">$28,888.88 <span>/mo</span></div>
        <ul class="lvl-features">
          <li>35,000 shipments/month</li>
          <li>Regional hub management</li>
          <li>Embedded finance access</li>
        </ul>
        <button class="lvl-btn">Select</button>
      </div>

      <div class="price-lvl">
        <div class="lvl-num">LEVEL 17</div>
        <div class="lvl-name">Intercontinental</div>
        <div class="lvl-price">$48,888.88 <span>/mo</span></div>
        <ul class="lvl-features">
          <li>60,000 shipments/month</li>
          <li>All 140 nodes included</li>
          <li>Board-level reporting</li>
        </ul>
        <button class="lvl-btn">Select</button>
      </div>

      <div class="price-lvl" style="border-color:var(--gold);background:linear-gradient(145deg,#1a1608,#211c08)">
        <div class="lvl-num" style="color:var(--gold)">LEVEL 18 — APEX</div>
        <div class="lvl-name" style="color:var(--gold)">Global Nexus</div>
        <div class="lvl-price" style="color:var(--gold)">$88,888.88 <span>/mo</span></div>
        <ul class="lvl-features">
          <li>Unlimited shipments</li>
          <li>Full platform white-label</li>
          <li>Blockchain trade settlement</li>
        </ul>
        <button class="lvl-btn" style="background:var(--gold);color:#000;border-color:var(--gold)">Contact Sales</button>
      </div>
    </div>
  </div>
</section>

<section class="sec bg-panel" id="payments">
  <div class="sec-hdr">
    <div>
      <div class="sec-ey">Secure Payment Gateway</div>
      <h2>4 Ways to Pay — Fast, Secure, Global</h2>
    </div>
  </div>

  <div class="pay-grid">
    <div class="pay-card bank">
      <div class="pay-icon">🏦</div>
      <div class="pay-title">Bank Transfer (SWIFT / SEPA)</div>
      <div class="pay-desc">Direct bank-to-bank wire transfer via SWIFT or SEPA. Settles within 1–3 business days.</div>
      <div class="pay-detail">
        <div class="pay-detail-row"><span class="pd-lbl">Account Name</span><span class="pd-val">Nexvoya Global Logistics Inc.</span></div>
        <div class="pay-detail-row"><span class="pd-lbl">SWIFT/BIC</span><span class="pd-val">NVXGSGSX</span></div>
        <div class="pay-detail-row"><span class="pd-lbl">IBAN (EUR)</span><span class="pd-val">NL88 NVXB 0001 4288 00</span></div>
      </div>
      <div class="pay-form">
        <label>Your Full Name / Company</label>
        <input class="pay-input" type="text" placeholder="e.g. Meridian Trading Ltd.">
        <label>Transfer Amount (USD)</label>
        <input class="pay-input" type="text" placeholder="e.g. $1,988.88">
      </div>
      <button class="pay-submit">Generate Bank Transfer Instructions</button>
      <div class="security-strip">256-bit encrypted · PCI DSS Level 1</div>
    </div>

    <div class="pay-card crypto">
      <div class="pay-icon">₿</div>
      <div class="pay-title">Cryptocurrency Payment</div>
      <div class="pay-desc">Pay natively in BTC, ETH, USDT, USDC, or BNB. Safe on-chain checkout pipeline.</div>
      <div class="pay-detail">
        <div class="pay-detail-row"><span class="pd-lbl">BTC Wallet</span><span class="pd-val">1NVX88...f4a2b8</span></div>
        <div class="pay-detail-row"><span class="pd-lbl">ETH / ERC-20</span><span class="pd-val">0x88Nex...9d4c</span></div>
      </div>
      <div style="margin-top:16px">
        <div class="pay-networks">
          <div class="pay-net">₿ Bitcoin</div>
          <div class="pay-net">Ξ Ethereum</div>
          <div class="pay-net">◎ USDT</div>
          <div class="pay-net">⬡ USDC</div>
        </div>
      </div>
      <div class="pay-form">
        <label>Select Currency</label>
        <select class="pay-input" style="cursor:pointer">
          <option>Bitcoin (BTC)</option>
          <option>Ethereum (ETH)</option>
          <option>Tether (USDT — TRC-20)</option>
        </select>
        <label>Amount in USD</label>
        <input class="pay-input" type="text" placeholder="e.g. $488.88">
      </div>
      <button class="pay-submit">Generate Crypto Invoice &amp; QR</button>
      <div class="security-strip">On-chain verified · AML screened</div>
    </div>

    <div class="pay-card card">
      <div class="pay-icon">💳</div>
      <div class="pay-title">Credit Card</div>
      <div class="pay-desc">Instant secure card processing configured with global standard multi-currency routing rules.</div>
      <div class="pay-networks" style="margin-bottom:18px">
        <div class="pay-net">VISA</div>
        <div class="pay-net">Mastercard</div>
        <div class="pay-net">Amex</div>
      </div>
      <div class="pay-form">
        <label>Cardholder Name</label>
        <input class="pay-input" type="text" placeholder="As printed on card">
        <label>Card Number</label>
        <input class="pay-input" type="text" placeholder="•••• •••• •••• ••••" maxlength="19">
        <div class="pay-row2">
          <div>
            <label>Expiry Date</label>
            <input class="pay-input" type="text" placeholder="MM / YY">
          </div>
          <div>
            <label>CVV / CVC</label>
            <input class="pay-input" type="text" placeholder="•••" maxlength="4">
          </div>
        </div>
      </div>
      <button class="pay-submit">Pay Securely Now</button>
      <div class="security-strip">3D Secure 2.0 Enabled · SSL Encrypted</div>
    </div>

    <div class="pay-card debit">
      <div class="pay-icon">🪙</div>
      <div class="pay-title">Debit Card</div>
      <div class="pay-desc">Deduct direct settlement balances from your local checking account structure immediately.</div>
      <div class="pay-networks" style="margin-bottom:18px">
        <div class="pay-net">Visa Debit</div>
        <div class="pay-net">MC Debit</div>
      </div>
      <div class="pay-form">
        <label>Cardholder Name</label>
        <input class="pay-input" type="text" placeholder="As printed on card">
        <label>Debit Card Number</label>
        <input class="pay-input" type="text" placeholder="•••• •••• •••• ••••" maxlength="19">
        <div class="pay-row2">
          <div>
            <label>Expiry Date</label>
            <input class="pay-input" type="text" placeholder="MM / YY">
          </div>
          <div>
            <label>CVV</label>
            <input class="pay-input" type="text" placeholder="•••" maxlength="3">
          </div>
        </div>
      </div>
      <button class="pay-submit">Confirm Debit Payment</button>
      <div class="security-strip">Bank-grade encryption · Fraud monitoring</div>
    </div>
  </div>
</section>

<section class="sec bg-steel" id="support">
  <div class="sec-hdr">
    <div>
      <div class="sec-ey">Global Support Team</div>
      <h2>We're Here Around the Clock</h2>
    </div>
  </div>

  <div class="support-grid">
    <div class="sup-card">
      <span class="sup-icon">💬</span>
      <div class="sup-title">Live Chat</div>
      <div class="sup-desc">Connect instantly with a specialist. Average response time under 90 seconds.</div>
      <a class="sup-btn" href="#">Start Live Chat →</a>
      <div class="sup-avail">Online now · 3 agents available</div>
    </div>

    <div class="sup-card">
      <span class="sup-icon">📞</span>
      <div class="sup-title">Phone Support</div>
      <div class="sup-desc">Available for Level 06 accounts and up. Multi-language infrastructure rules.</div>
      <a class="sup-btn" href="tel:+18884288880">+1 888 428 8880 →</a>
      <div class="sup-avail">Mon–Fri 06:00–22:00 UTC</div>
    </div>

    <div class="sup-card">
      <span class="sup-icon">📧</span>
      <div class="sup-title">Email Support</div>
      <div class="sup-desc">Formal legal queries, documentation audits, and corporate custom SLA setups.</div>
      <a class="sup-btn" href="mailto:support@nexvoya.com">support@nexvoya.com →</a>
      <div class="sup-avail">SLA: 2h acknowledgement</div>
    </div>
  </div>

  <div class="contact-panel">
    <div>
      <div class="sec-ey" style="margin-bottom:10px">Send a Message</div>
      <h2 style="margin-bottom:24px;font-size:22px">Contact our Support Team</h2>
      <div class="cf-row2">
        <div>
          <label class="cf-label">First Name</label>
          <input class="cf-input" type="text" placeholder="John">
        </div>
        <div>
          <label class="cf-label">Last Name</label>
          <input class="cf-input" type="text" placeholder="Meridian">
        </div>
      </div>
      <label class="cf-label">Company / Organisation</label>
      <input class="cf-input" type="text" placeholder="Meridian Trading Ltd.">
      <label class="cf-label">Email Address</label>
      <input class="cf-input" type="email" placeholder="john@meridiantrading.com">
      <label class="cf-label">Subject</label>
      <select class="cf-input" style="cursor:pointer">
        <option>Shipment Tracking Query</option>
        <option>Payment &amp; Billing Issue</option>
        <option>Account Upgrade / Pricing</option>
        <option>Technical / API Support</option>
      </select>
      <label class="cf-label">Message</label>
      <textarea class="cf-textarea" rows="4" placeholder="Describe your query in detail."></textarea>
      <button class="cf-submit">Send Message →</button>
    </div>

    <div class="contact-info">
      <div class="ci-title">Direct Contact Details</div>
      <div class="ci-item">
        <div class="ci-ico">🌐</div>
        <div>
          <div class="ci-lbl">Global Headquarters</div>
          <div class="ci-val">One Nexvoya Tower, 88 Maritime Boulevard,<br>Singapore 018988</div>
        </div>
      </div>

      <div class="ci-item">
        <div class="ci-ico">📞</div>
        <div>
          <div class="ci-lbl">Main Phone Line</div>
          <div class="ci-val"><a href="tel:+6568888880">+65 6888 8880</a> — Singapore HQ</div>
        </div>
      </div>

      <div class="ci-item">
        <div class="ci-ico">📧</div>
        <div>
          <div class="ci-lbl">Email Addresses</div>
          <div class="ci-val">
            <a href="mailto:support@nexvoya.com">support@nexvoya.com</a><br>
            <a href="mailto:sales@nexvoya.com">sales@nexvoya.com</a>
          </div>
        </div>
      </div>

      <div class="team-strip">
        <div class="ts-label">Your dedicated support team</div>
        <div class="team-avatars">
          <div class="t-av" style="background:#1a3050">👩‍💼</div>
          <div class="t-av" style="background:#1a2840">👨‍💻</div>
          <div class="t-av" style="background:#1a3048">👩‍🔬</div>
        </div>
        <div class="team-note"><strong>14 specialists</strong> online · avg. response 88 seconds</div>
      </div>
    </div>
  </div>
</section>

<footer style="background:var(--navy);border-top:1px solid var(--border);padding:48px;display:grid;grid-template-columns:2fr 1fr 1fr 1fr;gap:40px">
  <div>
    <div style="display:flex;align-items:center;gap:10px;font-family:var(--ff-disp);font-size:18px;font-weight:800;color:var(--white);margin-bottom:14px">
      <div style="width:30px;height:30px;background:var(--teal);border-radius:7px;display:flex;align-items:center;justify-content:center;font-size:14px">⬡</div>
      Nex<span style="color:var(--teal)">voya</span>
    </div>
    <p style="font-size:13px;color:var(--slate);line-height:1.7;max-width:280px">The world's first decentralized logistics-commerce platform. Connecting 140+ port nodes across 6 continents.</p>
  </div>
  <div>
    <div style="font-family:var(--ff-disp);font-size:13px;font-weight:700;color:var(--white);margin-bottom:14px">Platform</div>
    <div style="display:flex;flex-direction:column;gap:9px">
      <a href="#store" style="font-size:13px;color:var(--slate);text-decoration:none">Store</a>
      <a href="#staking-yields" style="font-size:13px;color:var(--slate);text-decoration:none">Staking Matrix</a>
      <a href="#pricing" style="font-size:13px;color:var(--slate);text-decoration:none">Pricing Levels</a>
    </div>
  </div>
  <div>
    <div style="font-family:var(--ff-disp);font-size:13px;font-weight:700;color:var(--white);margin-bottom:14px">Services</div>
    <div style="display:flex;flex-direction:column;gap:9px">
      <a href="#" style="font-size:13px;color:var(--slate);text-decoration:none">Ocean Freight</a>
      <a href="#" style="font-size:13px;color:var(--slate);text-decoration:none">Air Freight</a>
    </div>
  </div>
  <div>
    <div style="font-family:var(--ff-disp);font-size:13px;font-weight:700;color:var(--white);margin-bottom:14px">Company</div>
    <div style="display:flex;flex-direction:column;gap:9px">
      <a href="#support" style="font-size:13px;color:var(--slate);text-decoration:none">Contact</a>
      <a href="#" style="font-size:13px;color:var(--slate);text-decoration:none">Privacy Policy</a>
    </div>
  </div>
</footer>
<div style="background:var(--navy);border-top:1px solid var(--border);padding:20px 48px;display:flex;justify-content:space-between;align-items:center;font-size:12px;color:var(--slate)">
  <span>© 2026 Nexvoya Global Logistics Inc. All rights reserved. UEN: 202688880G · Singapore</span>
  <span style="font-family:var(--ff-mono)">v4.18.88</span>
</div>

<div class="cyber-sentinel">
  <div class="radar-scope">
    <div class="radar-blip"></div>
    <div class="radar-blip"></div>
  </div>
  <div class="sentinel-info">
    <div class="sentinel-status">
      <div class="sentinel-pulse"></div>
      Spy Detector Active
    </div>
    <div class="sentinel-log" id="radarLog">Scanning memory clusters...</div>
  </div>
</div>

<script>
// ── GLOBE ENGINE ──
(function(){
  const cv=document.getElementById('globe');if(!cv)return;
  const ctx=cv.getContext('2d');
  const W=680,H=680,R=280,cx=W/2,cy=H/2;
  let angle=0,t=0;
  const cities=[[31.2,121.5,'SHA'],[51.9,4.5,'RTM'],[1.3,103.8,'SIN'],[33.9,-118.4,'LAX'],[40.7,-74,'NYC'],[51.5,-0.1,'LHR'],[25.2,55.4,'DXB'],[35.6,139.7,'TYO'],[-4,39.7,'MBA'],[19.1,72.9,'BOM'],[-33.9,151.2,'SYD'],[48.9,2.3,'CDG']];
  const routes=[[0,1],[0,2],[0,3],[1,5],[2,3],[3,4],[4,5],[5,6],[6,7],[7,2],[2,8],[8,1],[9,2],[10,3],[11,5]];
  function p3d(lat,lng,rot){const φ=lat*Math.PI/180,λ=(lng+rot)*Math.PI/180;return{x:Math.cos(φ)*Math.sin(λ),y:-Math.sin(φ),z:Math.cos(φ)*Math.cos(λ)}}
  function proj(p){return{x:cx+p.x*R,y:cy+p.y*R,vis:p.z>0}}
  function draw(){
    ctx.clearRect(0,0,W,H);
    const g=ctx.createRadialGradient(cx,cy,0,cx,cy,R);
    g.addColorStop(0,'rgba(0,212,184,.05)');g.addColorStop(1,'rgba(0,212,184,0)');
    ctx.fillStyle=g;ctx.beginPath();ctx.arc(cx,cy,R,0,Math.PI*2);ctx.fill();
    ctx.beginPath();ctx.arc(cx,cy,R,0,Math.PI*2);ctx.strokeStyle='rgba(0,212,184,.14)';ctx.lineWidth=1;ctx.stroke();
    for(let lat=-60;lat<=60;lat+=30){const φ=lat*Math.PI/180,r=Math.cos(φ)*R,yy=cy-Math.sin(φ)*R;if(r>0){ctx.beginPath();ctx.ellipse(cx,yy,r,r*.18,0,0,Math.PI*2);ctx.strokeStyle='rgba(0,212,184,.07)';ctx.lineWidth=1;ctx.stroke()}}
    for(let lng=0;lng<360;lng+=30){const λ=(lng+angle)*Math.PI/180;ctx.beginPath();for(let i=0;i<=60;i++){const φ=(-90+i*3)*Math.PI/180,x=cx+Math.cos(φ)*Math.sin(λ)*R,y=cy-Math.sin(φ)*R;i===0?ctx.moveTo(x,y):ctx.lineTo(x,y)}ctx.strokeStyle='rgba(0,212,184,.05)';ctx.lineWidth=1;ctx.stroke()}
    routes.forEach(([ai,bi])=>{const a3=p3d(cities[ai][0],cities[ai][1],angle),b3=p3d(cities[bi][0],cities[bi][1],angle);if(a3.z<-.3&&b3.z<-.3)return;const ap=proj(a3),bp=proj(b3);if(!ap.vis&&!bp.vis)return;const mx=(ap.x+bp.x)/2,my=(ap.y+bp.y)/2,cpx=mx+(cx-mx)*.25,cpy=my+(cy-my)*.25;ctx.beginPath();ctx.moveTo(ap.x,ap.y);ctx.quadraticCurveTo(cpx,cpy,bp.x,bp.y);ctx.strokeStyle='rgba(0,212,184,.2)';ctx.lineWidth=1.2;ctx.stroke()});
    const pi=Math.floor(t)%routes.length,fr=t%1,[ai2,bi2]=routes[pi];
    const a3=p3d(cities[ai2][0],cities[ai2][1],angle),b3=p3d(cities[bi2][0],cities[bi2][1],angle);
    if(a3.z>-.2||b3.z>-.2){const ap2=proj(a3),bp2=proj(b3),mx=(ap2.x+bp2.x)/2,my=(ap2.y+bp2.y)/2,cpx=mx+(cx-mx)*.25,cpy=my+(cy-my)*.25,tt=fr,ot=1-tt,px=ot*ot*ap2.x+2*ot*tt*cpx+tt*tt*bp2.x,py=ot*ot*ap2.y+2*ot*tt*cpy+tt*tt*bp2.y,g2=ctx.createRadialGradient(px,py,0,px,py,8);g2.addColorStop(0,'rgba(0,212,184,.9)');g2.addColorStop(1,'rgba(0,212,184,0)');ctx.fillStyle=g2;ctx.beginPath();ctx.arc(px,py,8,0,Math.PI*2);ctx.fill();ctx.fillStyle='#00D4B8';ctx.beginPath();ctx.arc(px,py,2.5,0,Math.PI*2);ctx.fill()}
    cities.forEach(([lat,lng,lbl])=>{const p=p3d(lat,lng,angle);if(p.z<0)return;const pp=proj(p);ctx.beginPath();ctx.arc(pp.x,pp.y,3.5,0,Math.PI*2);ctx.fillStyle='#00D4B8';ctx.fill();ctx.fillStyle='rgba(248,250,252,.55)';ctx.font='10px JetBrains Mono,monospace';ctx.fillText(lbl,pp.x+8,pp.y+4)});
    angle+=.12;t+=.012;requestAnimationFrame(draw);
  }
  draw();
})();

// ── STORE FILTER ──
function filterStore(cat,el){
  document.querySelectorAll('.stab').forEach(t=>t.classList.remove('active'));
  el.classList.add('active');
  document.querySelectorAll('.prod-card').forEach(c=>{
    if(cat==='all'||c.dataset.cat===cat){c.style.display='';c.style.animation='fadeIn .3s ease'}
    else{c.style.display='none'}
  });
}

// ── DYNAMIC INVESTMENT MATRIX LOGIC ──
const projectData = [
  { name: "Sentinel Shield Node (SSN)", sector: "Cybersecurity & Threat Intel", shortRate: 6.20, longRate: 11.40 },
  { name: "Nexus Core Corridor Ledger", sector: "Decentralized Infra (DePIN)", shortRate: 7.50, longRate: 14.10 },
  { name: "Global Freight Liquidity Pool", sector: "Tokenized Commodities", shortRate: 5.80, longRate: 10.95 },
  { name: "RWA Autonomous Letter of Credit", sector: "On-Chain Trade Finance", shortRate: 8.10, longRate: 15.60 }
];

const levelLimits = [
  { lvl: 1, min: 88.98, max: 499.99 },
  { lvl: 2, min: 500.00, max: 1999.99 },
  { lvl: 3, min: 2000.00, max: 4999.99 },
  { lvl: 4, min: 5000.00, max: 9999.99 },
  { lvl: 5, min: 10000.00, max: 19999.99 },
  { lvl: 6, min: 20000.00, max: 34999.99 },
  { lvl: 7, min: 35000.00, max: 59999.99 },
  { lvl: 8, min: 60000.00, max: 100000.00 }
];

let activeProjIdx = 0;
let activeTerm = 'short';
let activeLevel = 1;

function selectProject(idx, element) {
  document.querySelectorAll('.asset-item').forEach(item => item.classList.remove('active'));
  element.classList.add('active');
  activeProjIdx = idx;
  document.getElementById('wkName').innerText = projectData[idx].name;
  document.getElementById('wkSector').innerText = projectData[idx].sector;
  calculateReturns();
}

function setTerm(term) {
  activeTerm = term;
  document.getElementById('btnShort').classList.toggle('active', term === 'short');
  document.getElementById('btnLong').classList.toggle('active', term === 'long');
  calculateReturns();
}

function setSliderValue(val) {
  document.getElementById('levelSlider').value = val;
  updateSliderMetrics();
}

function updateSliderMetrics() {
  activeLevel = parseInt(document.getElementById('levelSlider').value);
  document.getElementById('currentLevelDisplay').innerText = "LEVEL " + activeLevel;
  
  const labels = document.querySelectorAll('.lvl-dot-label');
  labels.forEach((lbl, index) => {
    lbl.classList.toggle('active', (index + 1) === activeLevel);
  });

  const limits = levelLimits[activeLevel - 1];
  const inputEl = document.getElementById('principalInput');
  let currentVal = parseFloat(inputEl.value);
  
  if (isNaN(currentVal) || currentVal < limits.min || currentVal > limits.max) {
    inputEl.value = limits.min.toFixed(2);
  }
  calculateReturns();
}

function calculateReturns() {
  const inputEl = document.getElementById('principalInput');
  let amount = parseFloat(inputEl.value);
  
  if (isNaN(amount)) amount = 88.98;
  if (amount < 88.98) amount = 88.98;
  if (amount > 100000) amount = 100000;

  let correctLvl = 1;
  for (let i = 0; i < levelLimits.length; i++) {
    if (amount >= levelLimits[i].min && amount <= levelLimits[i].max) {
      correctLvl = levelLimits[i].lvl;
      break;
    }
  }
  
  if (correctLvl !== activeLevel) {
    activeLevel = correctLvl;
    document.getElementById('levelSlider').value = correctLvl;
    document.getElementById('currentLevelDisplay').innerText = "LEVEL " + activeLevel;
    const labels = document.querySelectorAll('.lvl-dot-label');
    labels.forEach((lbl, idx) => lbl.classList.toggle('active', (idx + 1) === activeLevel));
  }

  const proj = projectData[activeProjIdx];
  const baseRate = (activeTerm === 'short') ? proj.shortRate : proj.longRate;
  const tierPremiumBonus = (activeLevel - 1) * 0.15;
  const totalRate = baseRate + tierPremiumBonus;
  const projectedEarnings = amount * (totalRate / 100);

  document.getElementById('calcRate').innerText = totalRate.toFixed(2) + "%";
  document.getElementById('calcReturns').innerText = "$" + projectedEarnings.toLocaleString('en-US', {minimumFractionDigits: 2, maximumFractionDigits: 2});
}

// ── SECURITY HUD TELEMETRY SIMULATION ──
const logs = [
  "Encrypted Tunnel: Standardized", 
  "Checking sandbox environments...", 
  "No hidden tracking scripts found.", 
  "Anti-Phishing Shield: ACTIVE", 
  "Zero-knowledge proof verified.", 
  "Memory pool telemetry clean.", 
  "Security Audit status: Safe"
];
setInterval(() => {
  const logEl = document.getElementById('radarLog');
  if(logEl) logEl.innerText = logs[Math.floor(Math.random() * logs.length)];
}, 3500);

updateSliderMetrics();
</script>
</body>
</html>
