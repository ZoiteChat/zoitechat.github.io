---
layout: default
title:
description: ZoiteChat is a modern IRC client based on HexChat.
---

<div class="hero">
  <section class="card hero__left">
    <div class="kicker">Simple. Fast. Familiar.</div>
    <h1 class="h1">ZoiteChat</h1>
    <p class="lead">
      A clean IRC client based on the HexChat codebase.
      ZoiteChat started from <strong>HexChat {{ site.hexchat_base_version }}</strong> with the initial ZoiteChat codebase at <strong>{{ site.zoitechat_initial_version }}</strong>.
    </p>

    <div class="actions">
      <a class="btn btn--primary" href="{{ "/downloads" | relative_url }}">Get ZoiteChat</a>
      <a class="btn" href="{{ site.docs_url | relative_url }}">Documentation</a>
      <a class="btn" href="{{ site.repo_url }}">View on GitHub</a>
    </div>

    <div class="badges">
      <span class="badge">Flatpak</span>
      <span class="badge">Plugins</span>
      <span class="badge">Themes</span>
      <span class="badge">SASL / TLS</span>
    </div>
  </section>

  <aside class="card hero__right">
    <div class="kicker">Status</div>
    <h2 style="margin:.35rem 0 .6rem; font-size:1.15rem;">Flatpak notes</h2>
    <p class="lead" style="margin:0;">
      The Flatpak build is available, but the <strong>Python plugin currently breaks the client</strong>.
      A fix is in progress.
    </p>

    <hr />

    <div class="kicker">Quick links</div>
    <ul style="margin:.5rem 0 0; padding-left:1.15rem;">
      <li><a href="{{ "/news" | relative_url }}">Release notes</a></li>
      <li><a href="{{ site.docs_url | relative_url }}">Docs</a></li>
      <li><a href="{{ site.repo_url }}/issues">Issue tracker</a></li>
    </ul>
  </aside>
</div>

<div class="grid">
  <section class="card">
    <h3>Comfortable defaults</h3>
    <p>Channels, networks, logging, notifications, and sane UI behavior without a maze of settings.</p>
  </section>
  <section class="card">
    <h3>Built for real servers</h3>
    <p>Handles modern IRC features: TLS, SASL, IPv6, and the usual everyday network weirdness.</p>
  </section>
  <section class="card">
    <h3>Hackable</h3>
    <p>Plugin support and a codebase familiar to anyone who has ever poked at HexChat.</p>
  </section>
</div>

<hr />

<div class="card">
  <h2 style="margin:.1rem 0 .6rem;">What is ZoiteChat?</h2>
  <p style="margin:0; color:var(--muted);">
    ZoiteChat is an IRC client derived from HexChat. The goal is a small, dependable desktop client that stays out of your way,
    with modern packaging and predictable behavior.
  </p>
</div>
