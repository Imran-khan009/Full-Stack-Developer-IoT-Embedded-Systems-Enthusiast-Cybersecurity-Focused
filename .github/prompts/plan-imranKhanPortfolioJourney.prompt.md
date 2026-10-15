## Plan: Imran Khan Portfolio Journey

Portfolio ko aapki di hui 6-year journey ke mutabiq real, scrollable sections me update karna hai. Existing matte-black background, neon orange `#ff6a3d`, clean typography, animated canvas aur responsive feel preserve rahenge.

**Steps**
1. [index.html](index.html) me hero ko aapke exact title, role badge, headline, bio aur chaar stats ke saath update karna. Existing desktop/mobile navigation ko real section IDs se jorna; Skills nav ko maujooda technology strip par anchor karna.
2. Experience section me chaaron supplied roles aur descriptions add karna. Filters honge: All Experience, Technical & IoT Instruction, Freelance & Digital Agency, Engineering & Design. Pehle do roles Technical & IoT me, teesra Freelance me, aur chautha Engineering & Design me filter hoga. IoT Instructor card par VATT certification aur UNICEF Program badges rahenge.
3. Modal-only project showcase ko chaar-card Work & Repositories grid se replace karna, supplied descriptions aur stacks ke saath. Jahan real project photos/screenshots nahi hain, wahan har project ke liye clearly illustrative schematic-style visual banana; inhe real build ki documentary photos ke taur par represent nahi karna.
4. Grid ke neeche accessible “Explore Full GitHub & Project Archive” expand/collapse control aur compact repository, video demonstration, aur student lab-session list add karna. Individual repo buttons supplied GitHub profile par jayenge. Demo, video aur Drive URLs filhaal unavailable/pending dikhaye jayenge, fake `#` links nahi honge.
5. “Let’s Work Together” contact section me supplied Fiverr, Upwork, GitHub, LinkedIn, Facebook, Instagram, WhatsApp aur email links icon-led controls ke saath add karna. WhatsApp `+92 333 1244214` par direct chat kholega; outdated email/phone targets ko bhi replace karna.
6. [style.css](style.css) me existing colors, fonts aur component style rakhte hue sections, stats, filters, project visuals, archive aur contact controls style karna. Mobile par content stack hoga, tab controls overflow nahi karenge, aur canvas ke upar text/cards overlap nahi honge.
7. [script.js](script.js) me navigation ko real sections par scroll karwana, active section ko actual scroll se track karna, 240-frame canvas scroll animation ko chalaye rakhna, experience filters aur archive toggle implement karna. Obsolete modal wiring ko hataana ya sirf zarurat par retain karna.

**Relevant Files**
- [index.html](index.html) — hero, nav/drawer, experience, projects/archive aur contact markup.
- [style.css](style.css) — existing theme tokens, layout aur responsive rules; inhi patterns me naye sections.
- [script.js](script.js) — scroll/canvas mapping, active navigation, filters aur archive interaction.
- [resume.html](resume.html) — unchanged; scope portfolio page tak hai.
- [server.ps1](server.ps1) — browser verification ke liye local server.

**Verification**
1. Available ho to `node --check .\script.js` chalana.
2. `powershell -ExecutionPolicy Bypass -File .\server.ps1` se local site khol kar navigation aur canvas scroll animation check karna.
3. Har experience filter, All reset, archive keyboard/pointer toggle aur `aria-expanded` state test karna.
4. Social/contact URLs verify karna; pending destinations active links ki tarah behave na karein.
5. Desktop, tablet aur narrow mobile widths par overflow, clipping, text readability, card stacking aur nav drawer check karna.

**Decisions**
- Real page sections use honge, kyunki current page simulated scroll checkpoints aur modal-only Work/Contact flow par nirbhar hai.
- Career details aur social URLs aapke supplied content se hi aayenge; resume update scope me nahi hai.
- Repository links GitHub profile par ja sakte hain. Individual repo, live demo, video aur Drive URLs na milne tak unke actions pending rahenge.
- Project visuals illustrative schematics honge, real project photos ka daawa nahi karenge.
