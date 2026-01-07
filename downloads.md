---
layout: default
title: Downloads
---

<div class="card">
  <h1 style="margin:.1rem 0 .6rem;">Downloads</h1>
  <p class="lead" style="margin:0;">
    Releases are published on GitHub. Flathub packaging is planned, but not ready yet.
  </p>
</div>

<div class="grid grid--downloads" style="margin-top:1rem;">
  <section class="card">
    <h3>Releases (recommended)</h3>
    <p>Grab the latest release assets here:</p>
    <p style="margin-top:.6rem;">
      <a class="btn btn--primary" href="{{ site.repo_url }}/releases">Open ZoiteChat Releases</a>
    </p>
    <p class="muted" style="margin-top:.6rem;">
      Releases typically include a <code>.flatpak</code> bundle (Linux) and source tarballs.
    </p>
  </section>

  <section class="card">
    <h3>Manual Flatpak install</h3>
    <p>Download the <code>.flatpak</code> bundle from the Releases page, then install it locally:</p>
    <pre><code># 1) (one-time) ensure Flatpak is installed
#    (use your distro package manager)

# 2) (recommended) add Flathub so runtimes can be pulled automatically
flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo

# 3) install the downloaded bundle (example filename)
flatpak install --user ./io.github.Zoitechat.flatpak

# 4) run it
flatpak run io.github.Zoitechat</code></pre>
    <p class="muted"><strong>Known issue:</strong> the Python plugin currently freezes the client. Disable the Python plugin (or run with <code>--no-plugins</code>) until fixed.</p>
  </section>

  <section class="card">
    <h3>Documentation</h3>
    <p>The docs live here:</p>
    <p><a class="btn" href="{{ site.docs_url | relative_url }}">/docs/en/latest/</a></p>
  </section>
</div>

<div class="card" style="margin-top:1rem;">
  <h2 style="margin:.1rem 0 .6rem;">Flatpak troubleshooting</h2>
  <ul style="margin:.3rem 0 0; padding-left:1.1rem;">
    <li>Temporarily run without plugins: <code>flatpak run io.github.Zoitechat --no-plugins</code></li>
    <li>Inspect runtime permissions: <code>flatpak info --show-permissions io.github.Zoitechat</code></li>
    <li>Verbose logging: <code>G_MESSAGES_DEBUG=all flatpak run io.github.Zoitechat</code></li>
  </ul>
  <p class="muted" style="margin:.7rem 0 0;">
    Updating a locally installed bundle is simple: download the newer <code>.flatpak</code> from Releases and run the same <code>flatpak install</code> command again.
  </p>
</div>
