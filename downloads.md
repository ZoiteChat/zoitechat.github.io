---
layout: default
title: Downloads
---

<div class="card">
  <h1 style="margin:.1rem 0 .6rem;">Downloads</h1>
  <p class="lead" style="margin:0;">
    ZoiteChat is currently distributed primarily via Flatpak while the rest of the packaging story catches up.
  </p>
</div>

<div class="grid" style="margin-top:1rem;">
  <section class="card">
    <h3>Flatpak</h3>
    <p>Recommended on Linux. If you built a bundle, install it like this (Flathub packaging is planned).</p>
    <pre><code>flatpak install --user io.github.Zoitechat.flatpak
flatpak run io.github.Zoitechat</code></pre>
    <p class="muted"><strong>Known issue:</strong> the Python plugin currently freezes the client. Disable plugins or the Python plugin until fixed.</p>
  </section>

  <section class="card">
    <h3>Source</h3>
    <p>Build it yourself and help break things responsibly.</p>
    <pre><code>git clone {{ site.repo_url }}
cd zoitechat</code></pre>
    <p class="muted">See docs for build requirements and packaging notes.</p>
  </section>

  <section class="card">
    <h3>Documentation</h3>
    <p>The docs live here (and yes, it is supposed to be a boring URL):</p>
    <p><a class="btn" href="{{ site.docs_url | relative_url }}">/docs/en/latest/</a></p>
  </section>
</div>

<div class="card" style="margin-top:1rem;">
  <h2 style="margin:.1rem 0 .6rem;">Flatpak troubleshooting</h2>
  <ul style="margin:.3rem 0 0; padding-left:1.1rem;">
    <li>To temporarily run without plugins: <code>zoitechat --no-plugins</code></li>
    <li>To inspect runtime permissions: <code>flatpak info --show-permissions io.github.Zoitechat</code></li>
    <li>To run with verbose logging: <code>G_MESSAGES_DEBUG=all flatpak run io.github.Zoitechat</code></li>
  </ul>
</div>
