---
layout: page
title: Shatranj
description: Shatranj is an interface to play chess
img:
importance: 5
category: Fun
---

<div id="shatranj"></div>

<script>
const githubUser = "mmkarandikar";
const repoName = "chess_engine";
const branch = "main";

// 1. Fetch the HTML
fetch(`https://cdn.jsdelivr.net/gh/${githubUser}/${repoName}@${branch}/index.html`)
  .then(response => response.text())
  .then(html => {
    // 2. Inject into your page
    const container = document.getElementById('shatranj');
    container.innerHTML = html;
    
    // 3. Fix all resource paths (critical step!)
    const baseUrl = `https://cdn.jsdelivr.net/gh/${githubUser}/${repoName}@${branch}/`;
    
    // Fix CSS links
    container.querySelectorAll('link[rel="stylesheet"]').forEach(link => {
      link.href = link.href.replace(/(\.\.?\/)?frontend\//, baseUrl + 'frontend/');
    });
    
    // Fix script sources
    container.querySelectorAll('script[src]').forEach(script => {
      script.src = script.src.replace(/(\.\.?\/)?frontend\//, baseUrl + 'frontend/');
    });
    
    // Fix image paths (if any exist in your HTML)
    container.querySelectorAll('img[src]').forEach(img => {
      img.src = img.src.replace(/(\.\.?\/)?frontend\//, baseUrl + 'frontend/');
    });
  });
</script>