:root {
  --bg: #000000;
  --ink: #f2f2f2;
  --muted: #9a9a9a;
  --accent: #7dd3fc;
  --mark: #1e3a4a;
  --line: #262626;
  --card: #0d0d0d;
}

* { box-sizing: border-box; }

html { scroll-behavior: smooth; scroll-padding-top: 80px; }

body {
  margin: 0;
  background: var(--bg);
  color: var(--ink);
  font-family: "Bricolage Grotesque", system-ui, -apple-system, "Segoe UI", sans-serif;
  font-size: 1.05rem;
  line-height: 1.65;
}

a { color: var(--accent); }
a:focus-visible, .btn:focus-visible {
  outline: 3px solid var(--accent);
  outline-offset: 3px;
}

/* Header */
.top {
  position: sticky;
  top: 0;
  z-index: 10;
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  gap: 0.5rem 1.5rem;
  padding: 0.9rem 1.5rem;
  background: var(--bg);
  border-bottom: 1px solid var(--line);
}
.logo { font-weight: 800; color: var(--ink); text-decoration: none; }
.top nav { display: flex; gap: 1.2rem; flex-wrap: wrap; }
.top nav a { color: var(--muted); text-decoration: none; font-weight: 600; }
.top nav a:hover { color: var(--accent); }

/* Layout */
main { max-width: 760px; margin: 0 auto; padding: 0 1.5rem; }
section { padding: 3.5rem 0; border-bottom: 1px solid var(--line); }
section:last-of-type { border-bottom: none; }

h2 { font-size: 1.7rem; margin: 0 0 1rem; letter-spacing: -0.01em; }

/* Hero */
.hero { padding: 5rem 0 4rem; }
.hello { margin: 0; color: var(--muted); font-size: 1.2rem; }
.hero h1 {
  margin: 0.2rem 0 1rem;
  font-size: clamp(3.2rem, 14vw, 6.5rem);
  line-height: 1;
  font-weight: 800;
  letter-spacing: -0.03em;
  background: linear-gradient(transparent 62%, var(--mark) 62%);
  display: inline-block;
}
.role { max-width: 34rem; font-size: 1.2rem; color: var(--muted); }

.actions { display: flex; gap: 0.8rem; flex-wrap: wrap; margin-top: 1.8rem; }
.btn {
  display: inline-block;
  padding: 0.7rem 1.3rem;
  border: 2px solid var(--ink);
  border-radius: 8px;
  color: var(--ink);
  font-weight: 600;
  text-decoration: none;
}
.btn:hover { background: var(--ink); color: var(--bg); }
.btn.primary { background: var(--accent); border-color: var(--accent); color: #000; }
.btn.primary:hover { filter: brightness(0.85); }

/* Skills */
.chips { list-style: none; margin: 0; padding: 0; display: flex; flex-wrap: wrap; gap: 0.6rem; }
.chips li {
  padding: 0.4rem 1rem;
  border: 1.5px solid var(--line);
  border-radius: 999px;
  background: var(--card);
  font-weight: 600;
}

/* Education */
.timeline { list-style: none; margin: 0; padding: 0 0 0 1.2rem; border-left: 2px solid var(--line); }
.timeline li { position: relative; padding: 0 0 0.5rem 1rem; }
.timeline li::before {
  content: "";
  position: absolute;
  left: -1.72rem;
  top: 0.55rem;
  width: 12px;
  height: 12px;
  border-radius: 50%;
  background: var(--accent);
}
.when { display: block; color: var(--muted); font-size: 0.95rem; }

/* Footer */
footer {
  text-align: center;
  padding: 2rem 1rem;
  color: var(--muted);
  border-top: 1px solid var(--line);
}

@media (prefers-reduced-motion: reduce) {
  html { scroll-behavior: auto; }
}
